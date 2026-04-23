---
title: "Enable Data Translation for Custom Fields"
source: "https://help.salesforce.com/s/articleView?id=platform.data_translation_enable_custom_fields.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Enable Data Translation for Custom Fields

Enable Data Translation for Custom Fields[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Enable Data Translation for Custom Fields

Allow translation of data stored in custom fields on certain objects and fields. You can enable data translation on custom fields with a type of Text, Text Area, Text Area (Long), Text Area (Rich), and URL.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To change data translation settings: | 
Customize Application

AND

Modify All Data

 |

Before enabling data translation for custom fields, you must enable data translation.

Note Data translation requires API version 48.0 or later.

1.  From Setup, in the Quick Find box, enter Data Translation Settings, and then select **Data Translation Settings**.
2.  Select an object to enable data translation for its custom fields.
    
    Only objects that support data translation are listed.
    
3.  Select the custom fields that you want to make available for data translation.
    
    Data translation can only be enabled on custom fields with a type of Text, Text Area, Text Area (Long), Text Area (Rich), and URL.
    
4.  Click **Save**.

If your B2B Commerce Store supports multiple languages, data translation is available for the selected custom fields through the Translation tab within Product and Product Category. You can also manage your data translations through the Export and Import options within Translation Workbench.

#### See Also

-   [Salesforce B2B Commerce and D2C Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)
-   [Salesforce B2B Commerce and D2C Commerce Enable Data Translation](https://help.salesforce.com/s/articleView?id=commerce.comm_enable_data_translation.htm&language=en_US&type=5)
-   [Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.workbench.htm&language=en_US&type=5 "Use Translation Workbench to maintain translated values for metadata and data labels in your Salesforce org. Specify languages for translation and assign translators for each language. Manage translated values for any Salesforce supported language. Translators can maintain translations directly through the workbench, or you can export translation files for bulk translation imports.")
-   [Localize Record Alerts](https://help.salesforce.com/s/articleView?id=ind.record_alerts_localize.htm&language=en_US&type=5)
-   [Manage Objects’ Data Translations](https://help.salesforce.com/s/articleView?id=platform.ls_manage_data_translations.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo