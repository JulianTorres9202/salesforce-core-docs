---
title: "Multilingual Solutions Overview"
source: "https://help.salesforce.com/s/articleView?id=service.sol_translate.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Multilingual Solutions Overview

Multilingual Solutions Overview[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Legacy Service Features](https://help.salesforce.com/s/articleView?id=service.support_legacy.htm&language=en_US&type=5)

# Multilingual Solutions Overview

The multilingual solutions feature helps you translate solutions and solution categories into the languages supported by Salesforce so that customers and support reps can find answers to inquiries in the language with which they are most comfortable.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.legacy_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

Multilingual solutions can lower support costs by:

-   Improving customer satisfaction by answering inquiries in the languages preferred by customers
-   Deflecting unnecessary incoming calls by providing solutions in languages that are the most useful for customers
-   Managing inquiries in multiple languages from one location, anytime and anywhere

There are two types of solutions, a master solution and a translated solution. A master solution is a solution created in any language supported by Salesforce. A master solution can have zero or more translations associated with it, but it cannot be linked to another master solution. A translated solution is a solution that is translated into another language supported by Salesforce and associated with exactly one master solution. A translated solution can't have the same language as its master solution or any other translated solutions associated with that master solution. A translated solution can't have other translated solutions associated with it.

You can work with multilingual solutions from the following:

-   Solutions Tab: When creating a new solution, users can choose a language in which to write the solution from the Language picklist field. Once the solution is saved, it becomes a master solution. Users can then create a translated solution by clicking **New** on the Translated Solutions related list of the master solution detail page. When a master solution is modified, users can adjust the statuses of its translated solutions to indicate that they may need translating.
-   Cases Tab: When users search for relevant solutions on a case by entering keywords in the Solutions related list and clicking **Find Solution**, search results include solutions in all languages that have matching keywords. Alternatively, if suggested solutions is enabled for cases, users can click **View Suggested Solutions** to find relevant solutions in multiple languages if they share common words with the case.
-   Self-Service Portal: If multilingual solution search is enabled for your Self-Service portal, customers automatically view solution search results in their preferred language as specified in their Self-Service user information settings. Customers can also choose to view solution search results in a specific language or all supported languages via a language drop-down list. By default, the Login Page of your Self-Service portal displays in your organization's language.
-   Public Solutions: If multilingual solution search is enabled for your public solutions, customers can choose to view solution search results in a specific language or all supported languages via a language drop-down list. By default, public solutions display in your organization's language.
-   Solution Categories: Users with the “Manage Translation” permission can use the translation workbench to translate solution categories so that they display in the language of each user on the Solutions tab and in the preferred language of each customer on the Self-Service portal as specified in the customer's user settings. Solution categories are not translated for public solutions.
-   Reports: You can track translated solutions marked Out of Date by choosing the Translated Solutions report. Running this report also lists the title and details of translated solutions. You can also create a custom report for multilingual solutions using the Master and Translated Solutions report type.
-   List Views: You can see which translated solutions are marked Out of Date and may need translating by creating a custom list view on the Solutions tab and entering the following search criteria: “Out of Date equals True”.
-   Import: The Data Import Wizard includes options to import master and translated solutions and associate them with each other.

To learn more about enabling multilingual solutions, see [Enable Multilingual Solutions](https://help.salesforce.com/s/articleView?id=service.sol_enable_translate.htm&language=en_US&type=5 "You can turn on multilingual solutions so users have the ability to translate solutions into multiple languages.").

#### See Also

-   [Enable Multilingual Solutions](https://help.salesforce.com/s/articleView?id=service.sol_enable_translate.htm&language=en_US&type=5 "You can turn on multilingual solutions so users have the ability to translate solutions into multiple languages.")
-   [Categorize Solutions](https://help.salesforce.com/s/articleView?id=service.sol_category.htm&language=en_US&type=5 "Use solution categories to group similar solutions together. Each solution can belong to more than one category.")
-   [Create Solutions](https://help.salesforce.com/s/articleView?id=service.creating_solutions.htm&language=en_US&type=5 "You can create a solution from the sidebar or Solutions tab and while closing a case.")

Did this article solve your issue?

Let us know so we can improve!

YesNo