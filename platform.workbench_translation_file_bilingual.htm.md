---
title: "Bilingual Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_bilingual.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Bilingual Translation Files

Bilingual Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Bilingual Translation Files

Use the Bilingual file to review translations, edit existing translations, and add translations for labels or data that haven't been translated. One Bilingual file is generated for each translation language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

Note Salesforce recommends the XML Localization Interchange File Format (.xlf) for translation files. See Considerations for Working with Translation Files for tips on editing translation files and how to translate rich text field content.

## XML Localization Interchange File Format (.xlf) Bilingual Translation Files

Bilingual .xlf translation file content is organized into translation units. Translation units for translated labels contain a `target` tag with the translated value. Untranslated labels have a `source` tag, but no `target` tag.

Tell your translators:

-   For untranslated labels, add a `target` tag containing the translated value after the `source` tag.
-   If the label’s translation is out of date, replace the text in the `target` tag. Outdated labels have a value of `outOfDate="true"` within the `trans-unit` tag.
-   To delete a translation, replace the value in the `trans-unit`'s `target` tag with `&lt;&gt;`. When the Bilingual file is imported, the label reverts to its primary label value.
-   A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.
-   Deleting the data translated value for a record’s Name field can delete all of that record’s other translated values for that language. See Considerations for Working with Translation Files for more information.
-   When translating text in a rich text area field, don’t delete HTML tags such as `<p></p>` and `<b></b>`. If you remove those tags, the translated text can be truncated.

| Tag | Description | Edit Options |
| --- | --- | --- |
| `trans-unit` | Translation unit. Contains unique identifiers for the label, including the label’s id, maximum width, and out-of-date indicator. | Do not edit. |
| `source` | Label or text in the org’s default language. | Do not edit. |
| `target` | The current translation that is visible to end users selecting the target language as their personal language. | Enter the translated value. Add a target tag if needed. Replace a value with `&lt;&gt;` to delete the translation. |
| `note` | Description of the metadata label, if defined, in the source language. | Do not edit. Translatable field descriptions each have a separate `trans-unit` tag. |

For example, in an org with English as its default language, you build a new custom Business Hours field on the Account object. This label is untranslated.

Nickname, an existing custom field on the Account object, has a Spanish translated value of “Apodo.” You change the primary label on the Nickname field from “Nickname” to “Preferred Name.” This label is outdated.

Another existing custom Prior Reference Number field on the Account object has an incorrect Spanish translated value of “Número de consulta previa.” Although the translation isn’t out of date, it must be updated to “Número de referencia precedente.”

The Name field on a custom Widget object had a primary label of “SLK.” A translator misinterpreted this acronym and entered a Spanish translation of “Flojo.” Although the translation isn’t out of date, you want to revert the translation to the primary label.

Finally, a custom Number field on a custom Widget object had a primary label of “Number” and a Spanish translated value of “Número.” You update the primary label to “#” and want to remove the translated value.

The exported Bilingual .xlf translation file contains the following row in the OUTDATED AND UNTRANSLATED section.

```markup
<trans-unit id="CustomField.Account.Business_Hours.FieldLabel" maxwidth="40" size-unit="char" outOfDate="false">
    <source>Business Hours</source>
</trans-unit>
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char" outOfDate="true">
    <source>Preferred Name</source>
    <target>Apodo</target>
    <note>The name preferred by this person.</note>
</trans-unit>
<trans-unit id="CustomField.Account.Prior_Ref_No.FieldLabel" maxwidth="20" size-unit="char" outOfDate="false">
    <source>Prior Reference Number</source>
    <target>Número de consulta previa</target>
</trans-unit>
<trans-unit id="CustomField.Widget__c.Name.FieldLabel" maxwidth="20" size-unit="char" outOfDate="false">
    <source>SLK</source>
    <target>Seda</target>
</trans-unit>
<trans-unit id="CustomField.Widget__c.Number.FieldLabel" maxwidth="20" size-unit="char" outOfDate="true">
    <source>#</source>
    <target>Número</target>
</trans-unit>
```

To make the requested changes:

-   Add a `target` tag with the translated value to the new Business Hours field.
-   Update the translation values in the target tags for the Preferred Name and Prior Reference Number fields.
-   To delete the translation of the Widget object’s Name and Number fields, update the translation values in those target tags with `&lt;&gt;`. When this file is imported, those labels revert to the primary label values.
-   Don’t change the `outOfDate` tag values. When you import the translated file, labels with updated translations are marked as up to date.

```markup
<trans-unit id="CustomField.Account.Business_Hours.FieldLabel" maxwidth="40" size-unit="char" outOfDate="false">
    <source>Business Hours</source>
    <target>Horario de oficina</target>
</trans-unit>
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char" outOfDate="true">
    <source>Preferred Name</source>
    <target>Nombre preferido</target>
    <note>The name preferred by this person.</note>
</trans-unit>
<trans-unit id="CustomField.Account.Prior_Ref_No.FieldLabel" maxwidth="20" size-unit="char" outOfDate="false">
    <source>Prior Reference Number</source>
    <target>Número de referencia precedente</target>
</trans-unit>
<trans-unit id="CustomField.Widget__c.Name.FieldLabel" maxwidth="20" size-unit="char" outOfDate="false">
    <source>SLK</source>
    <target>&lt;&gt;</target>
</trans-unit>
<trans-unit id="CustomField.Widget__c.Number.FieldLabel" maxwidth="20" size-unit="char" outOfDate="true">
    <source>#</source>
    <target>&lt;&gt;</target>
</trans-unit>
```

## Salesforce Translation Format (.stf) Bilingual Translation Files

Note Salesforce doesn’t recommend the STF format for translation files. If you choose to use this format, we don’t recommend editing the file with Microsoft Excel. For more information and restrictions, see Considerations for Working with Translation Files.

Bilingual .stf translation file content is separated into translated labels and outdated or untranslated labels.

The TRANSLATED section of the .stf file contains text that has been translated and is up to date. When importing, four columns are expected for each label in this section: KEY, LABEL, TRANSLATION, and OUT OF DATE.

For this section, tell your translators:

-   To update a current translation, replace the value in the TRANSLATION column.
-   To delete a translation, replace the value in the TRANSLATION column with a left and right angle bracket pair (`<>`). When the file is imported, the label reverts to its primary label’s value.

| Column | Description | Edit Options |
| --- | --- | --- |
| KEY | Unique identifier for the label. | Do not edit. |
| LABEL | Label or text in the org’s default language. | Do not edit. |
| TRANSLATION | The current translation that is visible to end users selecting the target language as their personal language. | 
-   To edit a translation, replace the translated value.
-   To delete a translation, replace the translated value with `<>`.

 |
| OUT OF DATE | 

Indicates whether the source text has changed since the previous translation.

A dash (`-`) indicates that the translation is current.

 | Do not edit. |

The OUTDATED AND UNTRANSLATED section of the file contains labels changed after the label’s translation value was last updated and text that hasn't been translated. When importing, two columns are expected for each label in this section: KEY and LABEL.

For this section, tell your translators:

-   Replace the text in the LABEL column with new or updated translation values.
-   Delete any values in the TRANSLATED and OUT OF DATE columns.
-   Delete the corresponding columns in the OUTDATED AND UNTRANSLATED section.
-   To delete an outdated translation, replace the value in the LABEL column with a left and right angle bracket pair (`<>`). When the file is imported, the label reverts to its primary label’s value.
-   A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.
-   Deleting the data translated value for a record’s Name field can delete all of that record’s other translated values for that language. See Considerations for Working with Translation Files for more information.

| Column | Description | Edit Options |
| --- | --- | --- |
| KEY | Unique identifier for the label. | Do not edit. |
| LABEL | Label or text in the org’s default language. | Replace label text with new or updated translated values. |
| TRANSLATION | 
The current translation that is visible to end users selecting the target language as their personal language.

Untranslated labels don’t have a value in this column.

 | Delete this column and its contents when updating an out-of-date translation. |
| OUT OF DATE | 

Indicates whether the source text has changed since the previous translation.

An asterisk (`*`) indicates that the label is out of date. A change was made to the primary label and the translation hasn't been updated.

Untranslated labels don’t have a value in this column.

 | Delete this column and its contents when updating an out-of-date translation. |

For example, in an org with English as its default language, an existing custom Prior Reference Number field on the Account object has an incorrect Spanish translated value of “Número de consulta previa.” Although the translation isn’t out of date, it must be updated to “Número de referencia precedente.”

The Name field on a custom Widget object had a primary label of “SLK.” A translator misinterpreted this acronym and entered a Spanish translation of “Flojo.” Although the translation isn’t out of date, you want to revert the translation to the primary label.

You also build a new custom Business Hours field on the Account object. This label is untranslated.

Nickname, another existing custom field on the Account object, has a Spanish translated value of “Apodo.” You change the primary label on the Nickname field from “Nickname” to “Preferred Name.” This label is outdated.

Finally, a custom Number field on a custom Widget object had a primary label of “Number” and a Spanish translated value of “Número.” You update the primary label to “#” and want to remove the translated value.

The exported Bilingual .stf translation file contains these rows in the OUTDATED AND UNTRANSLATED section.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:45%" lwc-3eigj2skqo3=""><col style="width:23%" lwc-3eigj2skqo3=""><col style="width:22%" lwc-3eigj2skqo3=""><col style="width:10%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="4" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">------------------TRANSLATED-------------------</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">TRANSLATION</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">OUT OF DATE</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Prior_Ref_No.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Prior Reference Number</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Número de consulta previa</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">–</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Widget__c.Name.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">SLK</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Seda</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">–</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="4" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">------------------OUTDATED AND UNTRANSLATED-----------------</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">TRANSLATION</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">OUT OF DATE</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Business_Hours.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Business Hours</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Preferred Name</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Apodo</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">*</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Widget__c.Number.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">#</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Número</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">*</code></td></tr></tbody></table>

To make the requested changes:

-   In the TRANSLATED section, update translations by replacing the value in the TRANSLATION column. To delete the translation of the Widget object’s Name field, replace the TRANSLATION value with `<>`. When this file is imported, the label for that Number field reverts to its primary label value of SLK.
-   In the OUTDATED AND UNTRANSLATED section, replace the value in the LABEL column. Then remove the TRANSLATION and OUT OF DATE columns and their content for the Nickname field. To delete the translation of the Widget object’s Number field, replace the TRANSLATION value with `<>`. When this file is imported, the label for that Number field reverts to its primary label value of #.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:45%" lwc-3eigj2skqo3=""><col style="width:23%" lwc-3eigj2skqo3=""><col style="width:22%" lwc-3eigj2skqo3=""><col style="width:10%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="4" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">------------------TRANSLATED-------------------</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">TRANSLATION</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">OUT OF DATE</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Prior_Ref_No.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Prior Reference Number</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Número de referencia precedente</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">–</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Widget__c.Name.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">SLK</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">&lt;&gt;</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">–</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="4" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">------------------OUTDATED AND UNTRANSLATED-----------------</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Business_Hours.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Horario de oficina</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Nombre preferido</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Widget__c.Number.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">&lt;&gt;</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr></tbody></table>

Important Delete the TRANSLATION and OUT OF DATE columns only in the OUTDATED AND UNTRANSLATED section. Rows in that section must have exactly two columns of data to be imported. Rows in the TRANSLATED section must have exactly four columns of data to be imported.

#### See Also

-   [Considerations for Working with Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_considerations.htm&language=en_US&type=5 "Review some important considerations to ensure that your edited translation file can be successfully imported.")

Did this article solve your issue?

Let us know so we can improve!

YesNo