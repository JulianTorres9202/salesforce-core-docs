---
title: "Source Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_source.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Source Translation Files

Source Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Source Translation Files

Use the Source file to translate an organization's labels or data for the first time. The Source file contains labels for all of a Salesforce org's translatable metadata or data in the org's default language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

Note Salesforce recommends the XML Localization Interchange File Format (.xlf) for translation files. See Considerations for Working with Translation Files for tips on editing translation files and how to translate rich text field content.

To prepare the translation file for your translators:

-   Create one copy of the Source file for each language you’re translating into.
-   In the header of each Source file, change the language code from the organization's default language to the translation language. For example, replace `en_US` for English (US) with `es` for Spanish.
-   Ensure that the headers are in the organization’s default language. To confirm, export a translation file and copy the headers.

## XML Localization Interchange File Format (.xlf) Source Translation Files

Source .xlf translation file content is organized into translation units. Translation units for translated labels contain a `target` tag with the translated value. Untranslated labels have a `source` tag, but no `target` tag.

Tell your translators:

-   After each `source` tag, add a `target` tag that contains the translated value.
-   If a `target` tag exists and the translation is out of date, replace the text in the target tag. Outdated labels have a value of `outOfDate="true"` within the trans-unit tag.
-   When translating text in a rich text area field, include all HTML tags such as `<p></p>` and `<b></b>`.

Important A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.

| Tag | Description | Edit Options |
| --- | --- | --- |
| `trans-unit` | Translation unit. Contains unique identifiers for the label, including the label’s id, maximum width, and out-of-date indicator. | Do not edit. |
| `source` | Label or text in the org’s default language. | Do not edit. |
| `target` | The current translation that’s visible to end users selecting the target language as their personal language. | Enter the translated value. Add a target tag if needed. |
| `note` | Description of the metadata label, if defined in the source language. | Do not edit. Translatable field descriptions each have a separate `trans-unit` tag. |

For example, if you build a custom Nickname field on the Account object, the original file contains this `trans-unit` tag in the exported Source .xlf file.

```markup
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char">
    <source>Nickname</source>
    <note>The person’s nickname, or what they prefer to be called.</note>
</trans-unit>
```

To translate this label, add a `target` tag containing the translated value to the corresponding `trans-unit` tag after the `source` tag.

```markup
<trans-unit id="CustomField.Account.Nickname.FieldLabel" maxwidth="40" size-unit="char">
    <source>Nickname</source>
    <target>Apodo</target>
    <note>The person’s nickname, or what they prefer to be called.</note>
</trans-unit>
```

[](https://help.salesforce.com/s?language=en_US)

## Salesforce Translation Format (.stf) Source Translation Files

Note Salesforce doesn’t recommend the STF format for translation files. If you choose to use this format, we don’t recommend editing the file with Microsoft Excel. For more information and restrictions, see Considerations for Working with Translation Files.

[](https://help.salesforce.com/s?language=en_US)Tell your translators to replace the untranslated values in the LABEL column with translated values.

Important A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.

| Column | Description | Edit Options |
| --- | --- | --- |
| KEY | Unique identifier for the label. | Do not edit. |
| LABEL | Label or text in the org’s default language. | Replace untranslated values with translated values. |

For example, if you build a custom Nickname field on the Account object, the original file contains this row in the exported Source .stf file.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Nickname</code></td></tr></tbody></table>

To translate this label, replace the LABEL text in that row with the translated value.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3=""># KEY</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">LABEL</code></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">CustomField.Account.Nickname.FieldLabel</code></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><code lwc-3eigj2skqo3="">Apodo</code></td></tr></tbody></table>

Important Don't add columns to or remove columns from the .stf translation file.

#### See Also

-   [Considerations for Working with Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_considerations.htm&language=en_US&type=5 "Review some important considerations to ensure that your edited translation file can be successfully imported.")
-   [Supported Languages](https://help.salesforce.com/s/articleView?id=xcloud.faq_getstart_what_languages_does.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo