---
title: "Flow Translation Best Practices"
source: "https://help.salesforce.com/s/articleView?id=platform.flow_considerations_salesforce_features_translation.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Flow Translation Best Practices

Flow Translation Best Practices[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Automate Your Business Processes](https://help.salesforce.com/s/articleView?id=platform.platform_automation.htm&language=en_US&type=5)

# Flow Translation Best Practices

When you use Translation Workbench to translate flows, note these best practices.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a title="Learn about the editions and user interfaces that support Flow Builder. Some Flow Builder features integrate with other Salesforce products that require additional licenses." href="https://help.salesforce.com/s/articleView?id=platform.flow_ref_supported_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions.</a></td></tr></tbody></table>

-   Keep your labels as short as possible. The translated label can’t exceed 1,000 characters (or 255 characters for definition name and version name). If you have a long label for a display text field, consider breaking it up into multiple fields.
    
    Note Each use of a merge field in a label reduces the 1,000-character limit by 66 characters. For example, even though `{!Account.Name}` is only 15 characters long, it counts as 66 characters toward the limit.
    
-   When updating a primary label, check whether it has translations, and update as needed.
-   Avoid text templates when translating an email body or other formatted block text.
-   Avoid using logic that references translated values.

#### See Also

-   [_Salesforce Help_: Considerations for Translating Flows](https://help.salesforce.com/s/articleView?id=platform.workbench_flow_considerations.htm&language=en_US&type=5)
-   [Translate Flow Screen Components](https://help.salesforce.com/s/articleView?id=platform.flow_translate.htm&language=en_US&type=5 "To use multilingual labels for most flow screen components, use Translation Workbench. Flow screen components in beta and some generally available flow screen components don’t support this functionality. For those generally available flow screen components, use the $Label global variable to specify custom labels. You must create the custom labels before referencing them in a flow.")

Did this article solve your issue?

Let us know so we can improve!

YesNo