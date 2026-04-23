---
title: "Translating Salesforce CPQ Records"
source: "https://help.salesforce.com/s/articleView?id=sales.cpq_localization_concept.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translating Salesforce CPQ Records

Translating Salesforce CPQ Records[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce CPQ](https://help.salesforce.com/s/articleView?id=sales.cpq_master.htm&language=en_US&type=5)

# Translating Salesforce CPQ Records

You can specify which parts of key CPQ objects are translated. When you translate a record, you define the text fields’ translated values only for that record. That way you can have different translations for unique records across the same object. Salesforce CPQ stores the translated values in a localization record. (Salesforce CPQ Managed Package)

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce CPQ Winter ’16 and later</td></tr></tbody></table>

You can provide translated values for most of the Salesforce CPQ UI with the translation workbench or by defining custom labels.

-   Use the translation workbench for all custom field names, picklist values, and help messages. Salesforce CPQ translates values based off the User record's user locale. When Salesforce CPQ creates a quote document while translations are active, it evaluates the User record's user language instead to translate merge field values.
-   Define custom labels for button names and error messages.
-   Rename tabs and labels.

For all text fields on the following CPQ objects, use the Salesforce CPQ translation process to define a translated value.

-   Line Column
-   Price Dimension
-   Product
-   Product Feature
-   Product Option
-   Quote Template
-   Quote Term

Associate a language with a translated value for text fields on your record. You can define translations in any language that Salesforce supports. When a user of that language views the fields in the following locations, the translated values are shown.

-   Quote Line Editor
-   Order Product Selection page
-   PDF documents, if the user generated the document in the same language as an existing translation
    
    Note
    
    -   If the org language and PDF document language are the same, Salesforce CPQ doesn’t load translations on the PDF.
    -   In the quote line editor, segmented line editor fields don’t show overwritten label values from the Translation Workbench.
    -   If a quote line field exists in multiple field sets under different objects, the translation workbench under both objects must be saved. For example, if the quote line (QL) field SBQQ\_\_Optional\_\_c is added to the layout via the QL Segmented Line Item Drawer field set and the quote line group’s (QLG) Line Editor field set, Salesforce must override the labels for QL and QLG in the translation workbench.
    

-   **[Localize a CPQ Record](https://help.salesforce.com/s/articleView?id=sales.cpq_localize_a_record_task.htm&language=en_US&type=5)**  
    Define translations for text fields on certain types of CPQ objects. (Salesforce CPQ Managed Package)
-   **[Salesforce CPQ Localization Fields](https://help.salesforce.com/s/articleView?id=sales.cpq_localization_fields_ref.htm&language=en_US&type=5)**  
    When a user translates a record, Salesforce CPQ creates a localization record for each text field that you translated. Depending on your page layout and field-level security settings, some fields might not be visible. (Salesforce CPQ Managed Package)

Did this article solve your issue?

Let us know so we can improve!

YesNo