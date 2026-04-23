---
title: "Translation File IDs and Keys"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_keys.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translation File IDs and Keys

Translation File IDs and Keys[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Translation File IDs and Keys

Each translatable item has a unique identifier in the translation file. In .xlf files, it’s the id within a trans-unit tag. In .stf files, it’s the key. The structure of these identifiers differs for metadata and data translation files.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

Note Translation file keys and ids aren’t edited during translation. The text to be translated is in the translation file in the `source` tag for .xlf files or the label column for .stf files. For admins, knowing how the id or key work can help them understand how these identifiers are structured.

## Metadata Translation File IDs and Keys

All translatable metadata has a setup component. Depending on the setup component, the translatable metadata can have an object, aspect, custom report type entity, flow type, flow name, and flow component.

-   Metadata label translation file IDs and keys follow the format: SetupComponentName.ObjectName.AspectName.
-   Metadata label translation file IDs and keys for custom report types contain the report type entity in place of the object name. The format is: SetupComponentName.CustomReportEntityName.AspectName.
-   Metadata translation file IDs and keys for flows can also contain the flow component, flow type, flow name, flow version, flow screen, or flow aspect. See Flow Identifiers in Translation Files for detailed examples.

This table provides examples of metadata translation IDs and keys.

| Translation Label or Text | id (in .xlf Files) or Key (in .stf Files) |
| --- | --- |
| Country “Spain” in address | `AddressCountry.ES` |
| “Billing” button or link on the Account object | `ButtonOrLink.Account.Billing` |
| Label of the “Active” field on the Account object | `CustomField.Account.Active.FieldLabel` |
| Description of the “Active” field on the Account object | `CustomField.Account.Active.Description.FieldLabel` |
| Help text of the “Active” field on the Account object | `CustomField.Account.Active.Description.HelpText` |
| “Low” picklist entry in the Customer Priority picklist on the Account object | `PicklistValue.Account.CustomerPriority.Low` |
| Description of the “East Accounts” Custom Report Type | `CustomReportType.East_Accounts.Description` |
| “Accounts” Custom Report Type Layout Section on the “Accounts” Custom Report Type | `CrtLayoutSection.Custom_Accounts_Reports_1` |
| Description of the “Goal Layout” Custom Report Type Layout on the “Goals” Custom Report Type | `LayoutSection.Goal.Goal Layout.Description_1` |
| “Survey Customers” flow name | `Flow.​Flow.​Survey_​customers.​FieldLabel` |
| “Customer Name” screen input field on version 2 of the “Survey Customer” flow | `Flow.​Flow.​Survey_​customers.​2.​Survey_​Customer.​Field.​Customer_​Name.​FieldLabel` |

## Data Translation File IDs and keys

If data translation is enabled in your Salesforce org, the record ID is used to identify the translatable text in an exported data translation file. Data translation IDs and keys follow the format ObjectName.recordUniqueIdentifier.FieldName.

This table provides examples of data translation IDs and keys.

| Translation Label or Text | id (in .xlf Files) or Key (in .stf Files) |
| --- | --- |
| Name of the product with record ID `01txx0000006yvEAAQ` | `Product2.01txx0000006yvEAAQ.Name` |
| Description of the product with record ID `01txx0000006yvEAAQ` | `Product2.01txx0000006yvEAAQ.Description` |
| Text stored in a custom “Discount Notes” field for the product record ID `01txx0000006yvEAAQ` | `Product2.01txx0000006yvEAAQ.Discount_Notes__c` |

#### See Also

-   [Flow Components for Metadata Translation](https://help.salesforce.com/s/articleView?id=platform.workbench_flow_components.htm&language=en_US&type=5 "Flow components are the parts of a flow you can translate.")

Did this article solve your issue?

Let us know so we can improve!

YesNo