---
title: "Translate CPQ Quote Template Content"
source: "https://help.salesforce.com/s/articleView?id=sales.cpq_translate_template_content.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate CPQ Quote Template Content

Translate CPQ Quote Template Content[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce CPQ](https://help.salesforce.com/s/articleView?id=sales.cpq_master.htm&language=en_US&type=5)

# Translate CPQ Quote Template Content

Define translated values for the variables in your CPQ quote template content. You can define translations in any language that Salesforce supports. (Salesforce CPQ Managed Package)

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce CPQ Spring ’16 and later</td></tr></tbody></table>

1.  In the template content record you want to translate, click **Translate**.
2.  Select the language you want to translate your variables into.
3.  Complete these fields for each translation you want to make.
    1.  Variable Name: Enter your template content variable. Template content variables are written as `{!Text.VariableName}`.
    2.  Description: Enter a description of your translation.
    3.  Translated Value: Enter the translated value that your template content shows when you translate your quote document into your selected language.
4.  Click **Save** to store your translations and return to your template content record, or click **Quick Save** to save your translations and remain on the Translations page.
5.  To define translations for other languages, repeat steps 2 through 4.
6.  In your template content record, click **Edit**.
7.  Add your variables to your template content.

Example

Your company needs Spanish translations for their Quotation and QuoteNumber template content variables, so you define translations for these variables as follows.

Quotation

Variable Name: `{!template.Quotation__c}`

Definition: Label for Quotation

Translated Value: Cita de vente

QuoteNumber

Variable Name: `{!template.QuoteNumber__c}`

Definition: Quote Number

Translated Value: Numero de cita

The variable name on the Translations page must be the field’s API name without the `__c`. In this example, you would use `Quotation`.

Important

-   When you want to translate a quote document, make sure that you select a specific document language rather than **Default**. When you select **Default**, Salesforce CPQ shows only untranslated content. This process means that Salesforce CPQ doesn’t show user-translated template content such as merge fields and labels with variable translation values.
-   Picklist values aren’t translated when the picklist field is used in the Group Field of the quote template, even if the document language and user language are changed.

Did this article solve your issue?

Let us know so we can improve!

YesNo