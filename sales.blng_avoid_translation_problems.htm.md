---
title: "Avoid Translation Problems"
source: "https://help.salesforce.com/s/articleView?id=sales.blng_avoid_translation_problems.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Avoid Translation Problems

Avoid Translation Problems[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce Billing](https://help.salesforce.com/s/articleView?id=sales.blng_billing_parent.htm&language=en_US&type=5)

# Avoid Translation Problems

To avoid language translation problems when users change languages, override the translated labels. (Salesforce Billing Managed Package)

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: All Salesforce Billing Editions</td></tr></tbody></table>

1.  Log in to your org as a user whose language is to English.
2.  From Setup, in the Quick Find box, search for and select **Custom Labels**.
3.  Sort the custom labels by name.
4.  Use the alphabet list to go to the custom labels that start with C.
5.  Select **Calculation Proration Type Calendar Days** and override translations for all languages to calendar days.
6.  Select **Calculation Proration Type CPQ Month** and override translations for all languages to monthly (CPQ formula).
7.  In the Quick Find box, search for and select **Installed Packages**.
8.  Configure the Salesforce Billing installed package.
9.  From the Invoice tab, select a proration type value.
10.  Save the changes.
11.  Validate your setting for other updated languages.
     
     Upgrading a package can interrupt active APEX jobs. After you upgrade Salesforce Billing, check for failures in your active invoice runs, payment runs, and balance snapshots, and then restart the jobs where necessary.
     

Based on your company’s Salesforce Billing implementation, you must set up tax integration and payment gateway integrations.

#### See Also

-   [Tax Integrations](https://help.salesforce.com/s/articleView?id=sales.blng_tax_int.htm&language=en_US&type=5 "Send data from Salesforce Billing to an external tax calculation service. Tax integrations are the Salesforce Billing objects that define the relationship between your Salesforce Billing org and the external service you use for tax calculation. (Salesforce Billing Managed Package)")
-   [Processing Payments with Payment Gateways](https://help.salesforce.com/s/articleView?id=sales.blng_payment_gateways.htm&language=en_US&type=5 "Salesforce Billing supports payment interfaces to process credit card and ACH transactions. Payment gateways are external service providers that process these electronic payments. Salesforce Billing uses out-of-the-box or API integrations to interface with a payment gateway. (Salesforce Billing Managed Package)")

Did this article solve your issue?

Let us know so we can improve!

YesNo