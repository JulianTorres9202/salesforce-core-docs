---
title: "Considerations for Working with Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_considerations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Considerations for Working with Translation Files

Considerations for Working with Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Considerations for Working with Translation Files

Review some important considerations to ensure that your edited translation file can be successfully imported.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

## General Considerations

-   Translation files are identified with the .stf or .xlf extension. Don't change the file extension.
-   Salesforce recommends the XML Localization Interchange File Format (.xlf) for translation files.
-   All translation files are language-specific.
-   A translation file name includes the name of the export option used to create it, the language code for the file's content, and a date stamp. Data translation file names also include the name of the object.
-   Deleting a translation value, row, or `trans-unit` tag in the file doesn't remove the translation after the file is imported. To delete a translation, replace the translated text with `<>` in an .stf file or `&lt;&gt;` in an .xlf file. When the file is imported, the label reverts to its primary label value. See Outdated and Untranslated Translation Files and Bilingual Translation Files in Salesforce Help for examples.
    
    Note See the following Data Translation File Considerations for important notes about deleting the data translation for a record’s Name field.
    

## Exported Translation File Limits

-   When exporting metadata translation files, individual uncompressed files are limited to 5 MB each. If your org’s metadata translations exceed 5 MB, the system exports multiple files. If multiple .zip files are required, each file name is date-stamped and incremented. For example, Outdated and untranslated 2020–09–20 05:13\_part 1 of 2.zip.
-   Each data translation export request is limited to 1 GB of data and 100,000 records. If your requested export exceeds either of those limits, only a partial file is exported. To reduce the amount of data exported, use the language filter, available for the Outdated and translated and Bilingual export types. If your org’s data translations for a single object and language exceed either of those limits, use BULK API or [Data Loader](https://developer.salesforce.com/docs/atlas.en-us.dataLoader.meta/dataLoader/data_loader_intro.htm).
-   When exporting data translation files, individual uncompressed files are limited to 25 MB. If multiple files are required, each file name is date stamped and incremented. For example, Bilingual\_de\_Product2\_2020-10-20 0836\_1.xlf and Bilingual\_de\_Product2\_2020-10-20 0836\_2.xlf.

## Translation File Import Limits

-   When importing metadata translation files, individual uncompressed files are limited to 10 MB each.
-   If data translation isn’t enabled in your org, each imported .zip file is limited to 10 MB. If data translation is enabled, each imported .zip file is limited to 1 GB.
-   When importing data translation files, individual uncompressed files are limited to 50 MB each.
-   When zipping data translation files for import, each .zip file can contain up to 100,000 total translation records within up to 2 GB of uncompressed files.

## Data Translation File Considerations

A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.

When translating text in a rich text area field, don’t delete HTML tags such as `<p></p>` and `<b></b>`. If you remove those tags, the returned value of `toLabel(rich_text_area_field)` in SOQL queries can be truncated to 255 characters.

There are two ways to delete the translated values for all fields related to a record. Because translation files are language-specific, this action is per language.

Note You can restore deleted data translation values through the recycle bin.

-   Delete translated text for all of the record’s fields. For example, a Product has German translated values for its name and description. To remove all German data translations for that Product, replace the translated text for that Product record’s Name and Description fields with `<>` in an .stf file or `&lt;&gt;` in an .xlf file.
-   Delete the translated text for the record’s Name field, and remove the rows or `trans-unit` tags for the record’s other fields. For example, a Product has German translated values for its name and description. To remove all German data translations for that Product, replace the translated text for that Product record’s Name fields with `<>` in an .stf file or `&lt;&gt;` in an .xlf file. Also delete the row or `trans-unit` tag for that Product’s Description field.

If an imported translation file deletes the translated value for a record’s Name and includes a translated value for another field, no action is taken. For instance, you delete the translated value for a Product’s name but leave the translation key for that Product’s description unchanged in a translation file for German. When you import that translation file, no changes are made to that Product’s translated values for German.

## XML Localization Interchange File Format (.xlf) File Considerations

The .xlf format is the recommended export type because it contains more information than the .stf format, like the field width.

-   .xlf translation file content is organized into translation units. Translation units for translated labels contain a `target` tag with the translated value. Untranslated labels have a `source` tag, but no `target` tag.
-   Translators must create a `target` tag for each untranslated label to store the translated value. Otherwise, don't add tags to or remove tags from the .xlf file.
-   The `file` tag’s attributes define details about the translation file, such as the source language, target language, and the translation type.
-   The `trans-unit` tags’ attributes define details about the translation unit, such as the id and the field width.

## Salesforce Translation Format (.stf) File Considerations

The .stf format behaves like a .csv file, with content organized into tab-delimited columns.

-   If you don’t use a standard translation tool such as Trados, edit the file using an application that supports tabs and word wrap, such as WordPad.
-   Don't add columns to or remove columns from the translation file.
-   If you use tabs, new lines, or carriage returns in your text for translation, they’re represented with special characters in the .stf file format. Tabs are `\t`, new lines are `\n`, and carriage returns are `\r`. To ensure consistency between your language versions, ensure that these characters are maintained in your translations.
-   If you use Microsoft Excel to enter translations in an .stf file, your file format can be corrupted. MS Excel automatically adds quotation marks around entries that have commas. We recommend that you open your files in a text editor before importing them and remove these quotation marks. The import fails if these quotation marks aren’t removed.

## Translating Rich Text Fields

Fields with a type of Text Area (Rich) allow special formatting, such as bolding text or adding an image. When rich text fields are exported for translation, the translatable text for those fields includes encoded HTML tags.

If your translators edit raw translation files, make sure that they understand HTML tags and their encoding. When translating the text, HTML tags aren’t required. However, if HTML tags are included in a translated value, they must be valid and in the same format as the exported tags. If the tags are incorrect, the translation import fails.

Note The HTML tags are visible in the raw files. Many translation tools handle the conversion of markup languages like HTML for you.

All rich text field translations must be contained within an HTML paragraph (`<p>`) tag with the appropriate HTML encoding for that file type. If the translation value contains only plain text, the required paragraph tag is added upon import.

This table provides examples of exported rich text field content.

| Rich Text Field Content | Format | Exported Text |
| --- | --- | --- |
| Available in women’s shoe sizes 5–13. | .stf | `<p>Available in women’s shoe sizes 5-13.</p>` |
| .xlf | `&lt;p&gt;Available in women’s shoe sizes 5-13.&lt;/p&gt;` |
| 
15% discount available for veterans.

Verification required.

 | .stf | `<p>15% discount available for veterans. </p><p><b>Verification required.</b></p>` |
| .xlf | `&lt;p&gt;15% discount available for veterans. &lt;/p&gt;&lt;p&gt;&lt;b&gt;Verification required.&lt;/b&gt;&lt;/p&gt;` |
| 

Features:

-   Leather
-   Imported
-   Rubber sole
-   Lightweight
-   Flexible sole

 | .stf | `<p>Features:<ul><li>Leather</li><li>LImported</li><li>Rubber sole</li><li>Lightweight</li><li>Flexible sole</li></ul></p>` |
| .xlf | `&lt;p&gt;Features: &lt;ul&gt;&lt;li&gtLeather &lt;/li&gt&lt;li&gtImported &lt;/li&gt&lt;li&gtRubber sole &lt;/li&gt&lt;li&gtLightweight &lt;/li&gt&lt;li&gtFlexible sole &lt;/li&gt&lt;/ul&gt;&lt;/p&gt;` |
| See more information at [this reference site](https://www.example.com). | .stf | `<p>See more information at <a href=”https://www.example.com”>this reference site</a>.</p>` |
| .xlf | `&lt;p&gt;&lt;a href=&quot;https://www.example.com&quot;&gt;this reference site&lt;/a&gt;.&lt;/p&gt;` |

#### See Also

-   [Export Metadata Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export.htm&language=en_US&type=5 "To easily translate your metadata, create files for your translators that contain your Salesforce org’s translatable metadata. Examples of translatable metadata include custom field labels, report type names, and picklist values.")
-   [Export Data Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export_data.htm&language=en_US&type=5 "If data translation is enabled in your Salesforce org, you can create files for your translators that contain your org’s data translations. Examples of translatable data include B2B Commerce Product names and data stored in custom fields.")
-   [Import Translated Files](https://help.salesforce.com/s/articleView?id=platform.workbench_import.htm&language=en_US&type=5 "Import and update the translations for your Salesforce org’s metadata, such as custom fields, report types, and picklist values. Or import and update data translations, such as Product names. Typically, you export translation files from Salesforce, then send them to outside translators or a translation agency for bulk translation activities. You then import the translated files.")
-   [View, Restore, and Manage the Recycle Bin in Salesforce Classic](https://help.salesforce.com/s/articleView?id=xcloud.home_delete.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo