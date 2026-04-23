---
title: "Translate Custom Labels"
source: "https://help.salesforce.com/s/articleView?id=platform.cl_translate_edit.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Custom Labels

Translate Custom Labels[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Enhance Salesforce with Code](https://help.salesforce.com/s/articleView?id=platform.extend_code_overview.htm&language=en_US&type=5)

# Translate Custom Labels

Translations for custom labels determine what text to display for the label’s value when a user’s default language is the translation language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: both Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Developer</strong>, <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| Create, edit, or delete custom labels: | Customize Application |
| Create or override a translation: | 
Manage Translation

OR

View Setup and Configuration and be designated as a translator

 |

Note You can’t delete custom labels installed as part of a managed package, or that are referenced by Apex or a Visualforce page. You can only override the existing translations.

To translate custom labels from Translation Workbench, visit [Translate Metadata Labels](https://help.salesforce.com/s/articleView?id=platform.entering_translated_terms.htm&language=en_US&type=5) in Salesforce Help.

To translate custom labels from Setup, take these steps.

1.  From Setup, in the Quick Find box, enter Custom Labels, then select **Custom Labels**.
2.  Select the name of the custom label to open.
3.  In the Translations related list, click **New** to enter a new translation or **Edit** next to the language to change a translation.
4.  Select the Language you are translating into.
5.  In the Translation Text field, enter the translated value. This text overrides the value specified in the label's Value field when a user's default language is the translation language.
6.  Save your changes.

Note When you package an app that uses custom labels with translations, include the translations by explicitly packaging the desired languages.

#### See Also

-   [Create and Edit Custom Labels](https://help.salesforce.com/s/articleView?id=platform.cl_edit.htm&language=en_US&type=5 "Create custom labels that can be referenced from Apex classes, Visualforce pages, Lightning pages, or Lightning components to make an app multilingual.")
-   [Custom Labels](https://help.salesforce.com/s/articleView?id=platform.cl_about.htm&language=en_US&type=5 "Custom labels enable developers to create multilingual applications by automatically presenting information (for example, help text or error messages) in a user’s native language. Custom labels are custom text values that can be accessed from Apex classes, Visualforce pages, Lightning pages, or Lightning components. The values can be translated into any language Salesforce supports.")

Did this article solve your issue?

Let us know so we can improve!

YesNo