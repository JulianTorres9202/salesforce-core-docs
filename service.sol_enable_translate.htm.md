---
title: "Enable Multilingual Solutions"
source: "https://help.salesforce.com/s/articleView?id=service.sol_enable_translate.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Enable Multilingual Solutions

Enable Multilingual Solutions[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Legacy Service Features](https://help.salesforce.com/s/articleView?id=service.support_legacy.htm&language=en_US&type=5)

# Enable Multilingual Solutions

You can turn on multilingual solutions so users have the ability to translate solutions into multiple languages.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.legacy_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To enable multilingual solutions: | Customize Application |

Before you enable multilingual solutions:

-   Run solution reports to locate any existing solutions that are already translated and will need to be converted to translated solutions after you enable multilingual solutions.
    
    When multilingual solutions is enabled for the first time, all existing solutions automatically become master solutions. You can create translated solutions from master solutions by associating a master solution without any translated solutions with a master solution of a different language via the Master Solution lookup field.
    
-   Translate any existing solution categories.
    
    Translated solutions inherit the solution categories of their master solution. We recommend that you translate your solution categories before enabling multilingual solutions and then associate solutions with each other. This will help you associate solutions with the correct categories.
    

1.  From Setup, enter Solution Settings in the Quick Find box, then select **Solution Settings**.
2.  Click **Edit**.
3.  Select Enable Multilingual Solutions.
4.  Optionally, select Enable Multilingual Solution Search in Self-Service Portal and Enable Multilingual Solution Search for Public Knowledge Base to allow customers to view solution search results in a specific language or all supported languages via a language drop-down list.
5.  Click **Save**.
6.  Customize solution page layouts to include the Master Solution Title field, Master Solution Details field, Out-of-Date field, and the Translated Solutions related list. The Language picklist and Master Solution lookup fields are automatically added to solution page layouts when you enable multilingual solutions.
    
    You can make solution edit pages easier for users to translate multilingual solutions by setting the Detail Information section to two columns and placing the Master Solution Title and Master Solution Details fields alongside each other. Underneath those fields, place the Solution Title and Solution Details fields alongside each other so that users can effortlessly compare the master and translated solutions. Note that the Master Solution Title and Master Solution Details fields display only on the translated solution edit page.
    
7.  Set the field-level security settings of the Master Solution lookup field to editable for profiles or permission sets with the “Create” and “Edit” permissions on solutions.
    
    When the Master Solution lookup field is editable, users can associate translated solutions with master solutions.
    
    Field-level security is available in Professional, Enterprise, Unlimited, Performance, and Developer Editions.
    
8.  Set the field-level security settings of the Out of Date checkbox field to visible for all profiles or permission sets with the “Read” permission on solutions. Field-level security is available in Professional, Enterprise, Unlimited, Performance, and Developer Editions.
9.  As a best practice, add a long text area custom field to solutions called Translation Comments and include it on solution page layouts so that users can add any comments regarding the translation of the solution. Users should include a date with their comments so that other users can see when each comment was added.

You can deselect the Enable Multilingual Solutions checkbox at any time, but deselecting it removes all associations between master and translated solutions and automatically disables the Enable Multilingual Solution Search in Self Service Portal and Enable Multilingual Solution Search for Public Solutions settings. If you select the Enable Multilingual Solutions checkbox again, the associations between master and translated solutions are restored.

After enabling multilingual solutions:

-   Associate any existing translated solutions with the appropriate master solutions.
    
    You can do this manually using the Master Solution lookup field, or you can export a report of existing translated solutions and then import those solutions to associate them with a master solution. For each translated solution you import, include the 15 to 18 character Solution ID field of its master solution in a master solution column on your import file. To view the Solution ID field for master solutions, run the Translated Solution report. If you import solutions by mistake, you can use mass delete to remove them from your organization.
    

#### See Also

-   [Multilingual Solutions Overview](https://help.salesforce.com/s/articleView?id=service.sol_translate.htm&language=en_US&type=5 "The multilingual solutions feature helps you translate solutions and solution categories into the languages supported by Salesforce so that customers and support reps can find answers to inquiries in the language with which they are most comfortable.")
-   [Categorize Solutions](https://help.salesforce.com/s/articleView?id=service.sol_category.htm&language=en_US&type=5 "Use solution categories to group similar solutions together. Each solution can belong to more than one category.")

Did this article solve your issue?

Let us know so we can improve!

YesNo