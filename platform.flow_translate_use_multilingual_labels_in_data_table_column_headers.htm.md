---
title: "Use Multilingual Labels in Data Table Column Headers"
source: "https://help.salesforce.com/s/articleView?id=platform.flow_translate_use_multilingual_labels_in_data_table_column_headers.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Use Multilingual Labels in Data Table Column Headers

Use Multilingual Labels in Data Table Column Headers[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Automate Your Business Processes](https://help.salesforce.com/s/articleView?id=platform.platform_automation.htm&language=en_US&type=5)

# Use Multilingual Labels in Data Table Column Headers

Add your translated column headers to the Data Table component using custom labels.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a title="Learn about the editions and user interfaces that support Flow Builder. Some Flow Builder features integrate with other Salesforce products that require additional licenses." href="https://help.salesforce.com/s/articleView?id=platform.flow_ref_supported_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions.</a></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To open, edit, create, activate or deactivate a flow using all flow types, elements, and features available in Flow Builder, including Einstein and Agentforce for Flow: | Manage Flow |

Before you begin, create and translate your custom labels. From Setup, enter Custom Labels in the Quick Find box, and select **Custom Labels**.

1.  In a Data Table component, click **Configure Columns**.
2.  For Source Field, select the field to use for the column.
3.  Select **Custom column label**.
    
    A new Label field appears.
    
4.  In the new Label field, enter the resource that contains the custom label using the `{!$Label.customLabelName}` expression.
    
    The resource menu isn’t available in the Label field, so the expression must be entered instead of selected.
    
5.  Repeat these steps for each column that you want to use a custom label.

#### See Also

-   [_Salesforce Help_: Custom Labels](https://help.salesforce.com/s/articleView?id=platform.cl_about.htm&language=en_US&type=5)
-   [_Salesforce Help_: Considerations for Translating Flows](https://help.salesforce.com/s/articleView?id=platform.workbench_flow_considerations.htm&language=en_US&type=5)
-   [Translate Flow Screen Components](https://help.salesforce.com/s/articleView?id=platform.flow_translate.htm&language=en_US&type=5 "To use multilingual labels for most flow screen components, use Translation Workbench. Flow screen components in beta and some generally available flow screen components don’t support this functionality. For those generally available flow screen components, use the $Label global variable to specify custom labels. You must create the custom labels before referencing them in a flow.")

Did this article solve your issue?

Let us know so we can improve!

YesNo