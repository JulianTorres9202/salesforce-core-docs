---
title: "XLIFF File Format for Importing Commerce Translations"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_xliff_file_format_import_translations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# XLIFF File Format for Importing Commerce Translations

XLIFF File Format for Importing Commerce Translations[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# XLIFF File Format for Importing Commerce Translations

The Translation Workbench supports the XML Localization Interchange File Format (XLIFF) and Salesforce Translation File (STF) file formats.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

Salesforce recommends that you use the XLIFF format. You can export the metadata and data translation source files and use them as a template to enter the initial translation of your store’s metadata, and Product, Promotion, and Category data fields. See [Export Data Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export_data.htm&language=en_US&type=5).

Important To properly encode a translation file for import, save the XFILL file in UTF-8 format.

| Element | Purpose | Attributes |
| --- | --- | --- |
| `<trans-unit>` | Represents a translatable unit within the XLF file. This element is used to encapsulate the source text and its corresponding translation | 
`ID:` A unique identifier for the translation unit.

`Maxwidth:` The maximum width allowed for the translated text.

`Field Type:` The type of field being translated.

-   `SingleLineText:` A line of text. Use for short text fields such as names, titles, or labels.
-   `MultiLineText:` Multiple lines of text. Use for longer text fields such as descriptions, comments, or notes.
-   R`ichText:` Text that can include formatting, such as bold, italics, lists, and hyperlinks. Use for content that requires rich text formatting.
-   H`TML:` HTML content. This field type is used for fields that contain HTML code. Use HTML content for more complex formatting and structure.
-   `Picklist:` A picklist (dropdown) field. Use for fields where the user selects a value from a predefined list of options.
-   C`heckbox:` A checkbox field. Use for fields that capture a boolean value (true or false).
-   `Date:` A date field. Use for fields that capture date values.
-   `DateTime:` A date and time field. Use for fields that capture both date and time values.
-   N`umber:` A numeric field. Use for fields that capture numeric values, such as quantities or amounts.
-   `Currency:` A currency field. Use for fields that capture monetary values.
-   `Email:` An email address field. Use for fields that capture email addresses.
-   `Phone:` A phone number field. Use for fields that capture phone numbers.
-   `URL:` A URL field. Use for fields that capture web addresses

`size-unit:` The unit of measurement for the size attribute.

-   `char:` The size of the text in terms of the number of characters.
-   `word:` The size of the text in terms of the number of words.
-   `pixel:` The size of the text in terms of the number of pixels. Use for graphical user interfaces where space is measured in pixels.
-   `pt:` The size of the text in terms of typographic points. Use in print and digital typography.
-   e`m:` The size of the text relative to the current font size, used for scalable and responsive design.
-   `percent:` The size of the text as a percentage of a reference value. Use with flexible layouts.

 |
| `<source>` | The original text that needs to be translated. Can include HTML encoding or CDATA sections for formatting. | None |
| `<target>` | The translated version of the text found in the `<source>` element. | 

Doesn't have mandatory attributes but can include optional attributes to provide additional context or metadata about the translation. Some common attributes can include:

-   `<state>` Indicates the status of the translation. For example, `new, translated, reviewed, final`.
-   `<xml:langt>` Specifies the language of the translated text. Use standard language codes for this entry. For example, `en, fr, de`.

 |

## Tips for XLIFF File Management

-   Context Information: Help your translators with message translation by adding a `<note>` tag in the `<target>` that explains the content of the message.
    
    ```
    <trans-unit id=&quot;homepage.greeting&quot;>
          <source>Hello, world!</source>
          <target>Bonjour, le monde!</target>
          <note>This is a greeting message displayed on the homepage.</note>
         </trans-unit>
    ```
    
-   Handling Placeholders and Variables: If your source text includes placeholders or variables (for example {0}, %s), make sure the placeholders are preserved in the target text and clearly documented for translators.
    
    ```
    <trans-unit id=&quot;product.price&quot;>
          <source>The price is {0}.</source>
          <target>Le prix est {0}.</target>
          <note>{0} will be replaced with the actual price</note>
         </trans-unit>
    ```
    
-   Validation and Testing: Validate the XLF file to make sure it's well-formed and adheres to the XLIFF standard. Use XML validation tools or editors that support XLIFF validation. Test the translations in a staging environment to make sure they appear correctly and that there are no formatting or display issues.
-   Consistent Language Codes: Use standard language codes (for example, `en` for English, `fr` for French, `de` for German) consistently
    
    ```
    throughout the file. 
         xml
           <file source-language="en" target-language="fr" 
           datatype="plaintext" original="example.txt">
         </file>
    ```
    
-   Version Control and Backup: Keep version control and backups of your XLF files. This is important for tracking changes, rolling back if needed, and maintaining a history of translations.
-   Integration with Translation Management Systems (TMS): If you're using a Translation Management System (TMS), make sure that the XLF files are compatible with the TMS and that the import/export processes are well-defined.
-   Handling Special Characters: Use CDATA sections or escape special characters (for example, &, <\`, \`>) to avoid XML parsing errors.
    
    ```
    <trans-unit id=&quot;special.characters&quot;>
            <source><p>Click & learn more.</p></source>
            <target><p>Cliquez & apprenez plus.</p></target>
         </trans-unit>
    ```
    
-   Rich Text Formatting: Use CDATA sections to include rich text formatting (HTML tags) within the <source> and <target> elements to prevent XML parsing issues.
    
    ```
    <trans-unit id=&quot;rich.text&quot;>
            <source><p>Welcome to <b>Salesforce</b>!</p></source>
            <target><p>Bienvenue chez<b>Salesforce</b>!</p></target>
         </trans-unit>
    ```
    

Did this article solve your issue?

Let us know so we can improve!

YesNo