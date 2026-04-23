---
title: "Set Up Primary Article and Translation Side-By-Side View"
source: "https://help.salesforce.com/s/articleView?id=service.knowledge_primary_translation_comparison_view.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set Up Primary Article and Translation Side-By-Side View

Set Up Primary Article and Translation Side-By-Side View[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Service](https://help.salesforce.com/s/articleView?id=service.service_cloud.htm&language=en_US&type=5)

# Set Up Primary Article and Translation Side-By-Side View

Look at a translated article and do a side-by-side comparison with the primary language version of the article. Admins can add a primary article component to the page layout so authors can view the primary language version beside the translated article.

### Required Editions

Important Where possible, we changed noninclusive terms to align with our company value of Equality. We maintained certain terms to avoid any effect on customer implementations.

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:100%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in Salesforce Classic and Lightning Experience. <a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.service_editions_reference.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To set up: | Manage Salesforce Knowledge AND Manage Articles |
| To view articles: | Allow View Knowledge |

To set up Primary Version and Translated Article viewing:

1.  From Setup, select the **Object Manager** tab.
2.  From the Object Manager, select the **Knowledge** object. Then select the **Lightning Record Page**.
3.  Click **Edit**, which takes you to the **Lightning App Builder**.
4.  Create a Translations tab in the right column and name it, Translations.
5.  Drag the **Translation Primary Article** component onto the new Translations page.
6.  Set component visibility filters, as needed. For example, if you set the filter to Is Primary Language Equal False, then the primary article component doesn’t show up. When you are on the primary language record (and you are not viewing the same version of the article in both columns).
7.  Save and activate the page.

Did this article solve your issue?

Let us know so we can improve!

YesNo