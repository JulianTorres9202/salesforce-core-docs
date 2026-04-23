---
title: "Salesforce CPQ Localization Fields"
source: "https://help.salesforce.com/s/articleView?id=sales.cpq_localization_fields_ref.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Salesforce CPQ Localization Fields

Salesforce CPQ Localization Fields[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce CPQ](https://help.salesforce.com/s/articleView?id=sales.cpq_master.htm&language=en_US&type=5)

# Salesforce CPQ Localization Fields

When a user translates a record, Salesforce CPQ creates a localization record for each text field that you translated. Depending on your page layout and field-level security settings, some fields might not be visible. (Salesforce CPQ Managed Package)

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce CPQ Winter ’16 and later</td></tr></tbody></table>

Localization records store information for only 1 text field at a time.

## Localization Fields

Language

The language code that Salesforce CPQ uses for this translation. When users view a field that you’ve localized into this language, they see the value that you provided within one of the record’s text fields.

Salesforce CPQ supports translation into all languages that Salesforce core supports. When you provide a value for this field, use one of the following language codes.

-   Chinese (Simplified): zh\_CN
-   Chinese (Traditional): zh\_TW
-   Danish: da
-   Dutch: nl\_NL
-   English: en\_US
-   Finnish: fi
-   French: fr
-   German: de
-   Italian: it
-   Japanese: ja
-   Korean: ko
-   Norwegian: no
-   Portuguese (Brazil): pt\_BR
-   Russian: ru
-   Spanish: es
-   Spanish (Mexico): es\_MX
-   Swedish: sv
-   Thai: th

API Name

The API name of the field with the translated label

Label

The original translated label

Text

The user-defined translation for the label of a text field

Text Area

The user-defined translation for the label of a text area field

Long Text Area

The user-defined translation for the label of a long text area field

Rich Text Area

The user-defined translation for the label of a rich text area field

Did this article solve your issue?

Let us know so we can improve!

YesNo