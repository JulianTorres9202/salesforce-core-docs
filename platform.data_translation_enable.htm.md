---
title: "Enable Data Translation"
source: "https://help.salesforce.com/s/articleView?id=platform.data_translation_enable.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Enable Data Translation

Enable Data Translation[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Enable Data Translation

Allow translation of data stored in certain objects and fields.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To view company information: | View Setup and Configuration |
| To change company information: | Modify All Data |

Note Before enabling data translation, note these important considerations:

-   Data translation requires API version 48.0 or later.
-   Data translation counts against your Salesforce org’s storage limits.
-   Data translation is available on some objects and fields. For example, data translation is available on the Industries Record Alert, Product, and Product Category objects.

1.  From Setup, in the Quick Find box, enter Company Information, and then select **Company Information**.
2.  In the Organization Detail section, click **Edit**.
3.  Select **Enable Data Translation**.
4.  Click **Save**.
    
    Data translation is available for the Name and Description fields through the Translation tab within Product. You can also manage your data translations through the Export and Import options within Translation Workbench.
    

Optionally, enable data translation for custom fields.

#### See Also

-   [Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.workbench.htm&language=en_US&type=5 "Use Translation Workbench to maintain translated values for metadata and data labels in your Salesforce org. Specify languages for translation and assign translators for each language. Manage translated values for any Salesforce supported language. Translators can maintain translations directly through the workbench, or you can export translation files for bulk translation imports.")
-   [Salesforce B2B Commerce and D2C Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)
-   [Salesforce B2B Commerce and D2C Commerce Enable Data Translation](https://help.salesforce.com/s/articleView?id=commerce.comm_enable_data_translation.htm&language=en_US&type=5)
-   [Data and File Storage Allocations](https://help.salesforce.com/s/articleView?id=xcloud.overview_storage.htm&language=en_US&type=5)
-   [Localize Record Alerts](https://help.salesforce.com/s/articleView?id=ind.record_alerts_localize.htm&language=en_US&type=5)
-   [Manage Objects’ Data Translations](https://help.salesforce.com/s/articleView?id=platform.ls_manage_data_translations.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo