---
title: "Outdated and Untranslated Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_outdated.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Outdated and Untranslated Translation Files

Outdated and Untranslated Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Outdated and Untranslated Translation Files

Use the Outdated and untranslated file to translate labels or data that need translation. The file includes labels or data changed since the last translation and labels that haven't been translated. One Outdated and untranslated file is generated for each language. When multiple files are generated, they're exported to a .zip file containing a file for each translation language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

Note Salesforce recommends the XML Localization Interchange File Format (.xlf) for translation files. See Considerations for Working with Translation Files for tips on editing translation files and how to translate rich text field content.

When working with the Outdated and untranslated translation file, each entry needs a new translated value. Special values are used to delete an existing translation and revert the label to its original value.

## XML Localization Interchange File Format (.xlf) Outdated and Untranslated Translation Files

Outdated and untranslated .xlf translation file content is organized into translation units. Translation units for translated labels contain a `target` tag with the translated value. Untranslated labels have a `source` tag, but no `target` tag.

Tell your translators:

-   For untranslated labels, add a `target` tag containing the translated value after each `source` tag.
-   If the label’s translation is out of date, replace the text in the target tag. Outdated labels have a value of `outOfDate="true"` within the trans-unit tag. Don’t update the `outOfDate` value.
-   To delete a translation, replace the value in the label's target tag with `&lt;&gt;`. When the Bilingual file is imported, the label reverts to its original value.
-   A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.
-   Deleting the data translated value for a record’s Name field can delete all of that record’s other translated values for that language. See Considerations for Working with Translation Files for more information.
-   When translating text in a rich text area field, don’t delete HTML tags such as `<p></p>` and `<b></b>`. If you remove those tags, the translated text can be truncated.

| Tag | Description | Edit Options |
| --- | --- | --- |
| `trans-unit` | Translation unit. Contains unique identifiers for the label, including the label’s id, maximum width, and out-of-date indicator. | Do not edit. |
| `source` | Label or text in the org’s default language. | Do not edit. |
| `target` | The current translation that is visible to end users selecting the target language as their personal language. | Enter the translated value. Add a target tag if needed. |
| `note` | Description of the metadata label, if defined, in the source language. | Do not edit. Translatable field descriptions each have a separate `trans-unit` tag. |

For example, an existing Nickname field on the Account object has a Spanish translated value of “Apodo.” You change the primary label on the Nickname field from “Nickname” to “Preferred Name.” That label is now outdated. You also build a new custom Business Hours field on the Account object. The exported Outdated and untranslated .xlf translation file contains the following `trans-unit` tags.

```markup
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char" outOfDate="true">
    <source>Preferred Name</source>
    <target>Apodo</target>
    <note>The name preferred by this person.</note>
</trans-unit>
<trans-unit id="CustomField.Account.Business_Hours.FieldLabel" maxwidth="40" size-unit="char" outOfDate="false">
    <source>Business Hours</source>
</trans-unit>
```

To update the outdated label, update the text in the corresponding `target` tag. To translate the new field’s label, add a `target` tag containing the translated value to the corresponding `trans-unit` tag after the `source` tag. Don’t change the `outOfDate` tag values. When you import the translated file, labels with updated translations are marked as up to date.

```markup
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char" outOfDate="true">
    <source>Preferred Name</source>
    <target>Nombre preferido</target>
    <note>The name preferred by this person.</note>
</trans-unit>
<trans-unit id="CustomField.Account.Business_Hours.FieldLabel" maxwidth="40" size-unit="char" outOfDate="false">
    <source>Business Hours</source>
    <target>Horario de oficina</target>
</trans-unit>
```

To delete the Preferred Name label’s translation, update the translation value in the target tag with `&lt;&gt;`. When the file is imported, the label reverts to its original value.

```markup
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char" outOfDate="true">
    <source>Preferred Name</source>
    <target>&lt;&gt;</target>
    <note>The name preferred by this person.</note>
</trans-unit>
```

## Salesforce Translation Format (.stf) Outdated and Untranslated Translation Files

Note Salesforce doesn’t recommend the STF format for translation files. If you choose to use this format, we don’t recommend editing the file with Microsoft Excel. For more information and restrictions, see Considerations for Working with Translation Files.

Tell your translators to replace the values in the LABEL column with updated translated values.

-   To delete a translation, replace the desired value in the TRANSLATION column with a left and right angle bracket pair (<>). When the file is imported, the label reverts to its original value.
-   A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.
-   Deleting the data translated value for a record’s Name field can delete all of that record’s other translated values for that language. See Considerations for Working with Translation Files for more information.

| Column | Description | Edit Options |
| --- | --- | --- |
| KEY | Unique identifier for the label. | Do not edit. |
| LABEL | Label or text in the org’s default language. | Replace untranslated values with translated values. |

For example, an existing custom Nickname field on the Account object has a Spanish translated value of “Apodo.” You change the primary label on the Nickname field from “Nickname” to “Preferred Name.” That label is now outdated. You also build a new custom Business Hours field on the Account object. The exported Outdated and untranslated .stf translation file contains these rows.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Preferred Name</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Business_Hours.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Business Hours</code></td></tr></tbody></table>

To translate the new field’s label and update the existing label, replace the LABEL text in each row.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Nombre preferido</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Business_Hours.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Horario de oficina</code></td></tr></tbody></table>

To delete the Nickname field’s outdated translation of “Apodo,” replace the translation value in the LABEL column with `<>`. When the file is imported, the label reverts to its primary label value of “Preferred Name.”

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">&lt;&gt;</code></td></tr></tbody></table>

#### See Also

-   [Considerations for Working with Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_considerations.htm&language=en_US&type=5 "Review some important considerations to ensure that your edited translation file can be successfully imported.")

Did this article solve your issue?

Let us know so we can improve!

YesNo