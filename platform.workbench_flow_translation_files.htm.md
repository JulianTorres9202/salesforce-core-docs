---
title: "Flow Identifiers in Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.workbench_flow_translation_files.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Flow Identifiers in Translation Files

Flow Identifiers in Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Flow Identifiers in Translation Files

In a translation file exported from Translation Workbench, a unique key or trans-unit ID attribute identifies a flow metadata label.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

Flows follow a convention based on the flow label.

| Flow Component | Key or Trans-Unit ID | Example |
| --- | --- | --- |
| Flow Definition Name | Flow.​flowType.​flowUniqueName.​FieldLabel | Flow.​Flow.​Survey\_​customers.​FieldLabel |
| Flow Version Name | Flow.​flowType.​flowUniqueName.​versionNumber.​Name | Flow.​Flow.​Survey\_​customers.​1.​Name |
| **Screen** |
| Paused Message | Flow.​flowType.​flowUniqueName.​versionNumber.​Screen.​screenUniqueName.​PausedText | Flow.​Flow.​Survey\_​customers.​1.​Screen.​Greet\_Customer.​PausedText |
| Help Text | Flow.​flowType.​flowUniqueName.​versionNumber.​Screen.​screenUniqueName.​HelpText | Flow.​Flow.​Survey\_​customers.​1.​Screen.​Greet\_​Customer.​HelpText |
| **Screen Input Field** |
| Label | Flow.​flowType.​flowUniqueName.​versionNumber.​screenUniqueName.​Field.​fieldUniqueName.​FieldLabel | Flow.​Flow.​Survey\_​customers.​2.​Survey\_​Customer.​Field.​Customer\_​Name.​FieldLabel |
| Help Text | Flow.​flowType.​flowUniqueName.​versionNumber.​screenUniqueName.​Field.​fieldUniqueName.​HelpText | Flow.​Flow.​Survey\_​customers.​2.​Survey\_​Customer.​Field.​Customer\_​Name.​HelpText |
| Error Message | Flow.​flowType.​flowUniqueName.​versionNumber.​screenUniqueName.​Field.​fieldUniqueName.​ErrorMessage | Flow.​Flow.​Survey\_​customers.​2.​Survey\_​Customer.​Field.Customer\_​Name.​ErrorMessage |
| **Screen Output Field** |
| Display Text | Flow.​flowType.​flowUniqueName.​versionNumber.​screenUniqueName.​Field.​fieldUniqueName.Description | Flow.​Flow.​Survey\_​customers​.2.​Greet\_​Customer.​Field.​WelcomeMessage.​Description |
| **Choice** |
| Label | Flow.​flowType.​flowUniqueName.​versionNumber.​Choice.​choiceUniqueName.​FieldLabel | Flow.​Flow.​Survey\_​customers.​2.​Choice.​Participate\_​No.​FieldLabel |
| Error Message | Flow.​flowType.​flowUniqueName.​versionNumber.​Choice.​choiceUniqueName.​ErrorMessage | Flow.​Flow.​Survey\_​customers.​2.​Choice.​Participate\_​No.​ErrorMessage |
| Input Label | Flow.​flowType.​flowUniqueName.​versionNumber.​Choice.​choiceUniqueName.​InputLabel | Flow.​Flow.​Survey\_​customers.​2.​Choice.​Participate\_​No.​InputLabel |
| **Stages** |
| Stage Label | Flow.​flowType.​flowUniqueName.​versionNumber.​Stage.​stageUniqueName.​FieldLabel | Flow.​Flow.​Stages\_​Online\_​Purchase\_​Breadcrumbs.​1.​Stage.​Billing\_​Details.​FieldLabel |
| **Text Template** |
| Label | Flow.​flowType.​flowUniqueName.​versionNumber.​​TextTemplate.​texttemplateUniqueName.​FieldLabel | Flow.​Flow.​Survey\_​customers.​2.​TextTemplate.​ParticipantCity\_​FieldLabel |

#### See Also

-   [Work with Translation Files](https://help.salesforce.com/s/articleView?id=platform.translation_file_description.htm&language=en_US&type=5 "Translate metadata labels or data translation text, or review existing translations, with XML Localization Interchange File Format (.xlf) or Salesforce Translation Format (.stf) files.")
-   [Considerations for Translating Flows](https://help.salesforce.com/s/articleView?id=platform.workbench_flow_considerations.htm&language=en_US&type=5 "When you use Translation Workbench to translate flows, note these considerations.")

Did this article solve your issue?

Let us know so we can improve!

YesNo