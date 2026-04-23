---
title: "Enable Data Translation"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_enable_data_translation.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Enable Data Translation

Enable Data Translation[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Enable Data Translation

When you enable data translation, you can translate the data stored in your B2B store product, category, and promotion fields. You can also enable data translation for custom text and URL fields on the product and category objects.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

Note Data translation requires API version 48.0 or later. Data translation counts against your org’s storage limits.

1.  Enable data translation for the name and description fields on the product and category objects.
    1.  Click  at the top of the page, and then select **Setup**.
    2.  In the Quick Find box, enter Company Information, and select **Company Information**.
    3.  In the Organization Detail section, click **Edit**.
    4.  Select **Enable Data Translation**.
    5.  Save your changes.
2.  Enable data translation for custom fields.
    1.  Click  at the top of the page, and then select **Setup**.
    2.  In the Quick Find box, enter Data Translation Settings, and select **Data Translation Settings**.
    3.  Select the object. Only the objects that support data translation are listed.
    4.  Select the custom fields that you want to make available for data translation.
        
        You can enable data translation only for custom fields with a type of Text, Text Area, Text Area (Long), Text Area (Rich), or URL.
        
    5.  Save your changes.

#### See Also

-   [Manage Objects' Data Translations](https://help.salesforce.com/s/articleView?id=platform.ls_manage_data_translations.htm&language=en_US&type=5)
-   [Configure Salesforce for Global Stores](https://help.salesforce.com/s/articleView?id=commerce.comm_config_org_for_international.htm&language=en_US&type=5 "Make sure that your language, translation, and currency settings support B2B Commerce stores around the world.")
-   [Manually Localize Product, Category, and Promotion Data](https://help.salesforce.com/s/articleView?id=commerce.comm_create_data_translation.htm&language=en_US&type=5 "You can manually enter translated text for your B2B product and category names and descriptions. To translate promotion names and descriptions, you must use Translation Workbench. To perform bulk translations for product, category, or promotion data, use Translation Workbench.")

Did this article solve your issue?

Let us know so we can improve!

YesNo