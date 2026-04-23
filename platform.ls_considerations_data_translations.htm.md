---
title: "Considerations for Data Translation of Objects"
source: "https://help.salesforce.com/s/articleView?id=platform.ls_considerations_data_translations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Considerations for Data Translation of Objects

Considerations for Data Translation of Objects[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce Scheduler](https://help.salesforce.com/s/articleView?id=platform.ls_overview.htm&language=en_US&type=5)

# Considerations for Data Translation of Objects

Here are some things to keep in mind when you translate object data.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience.</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong> and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</td></tr></tbody></table>

-   Administrators who implement their own screens by using Scheduler APIs and custom SOQLs can translate data of objects. Out-of-the-box screens aren’t supported.
-   Data translation is supported for these objects and fields:
    
    -   Name and Description fields for service resource, service territory, and work type group.
    -   Custom fields defined on the object service resource, service territory, and work type group that are of type Text, Text Area, Text Area (Long), Text Area (Rich), and URL.
    
    The Address field appears in the org’s default language and can’t be translated.
    

Did this article solve your issue?

Let us know so we can improve!

YesNo