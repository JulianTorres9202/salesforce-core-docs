---
title: "Manage Secondary Language Translations"
source: "https://help.salesforce.com/s/articleView?id=service.bots_service_language_translations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Manage Secondary Language Translations

Manage Secondary Language Translations[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Manage Secondary Language Translations

Edit bot translations directly in each bot dialog.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.einstein_service_intro.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To build and manage Einstein Bots: | 
Customize Application

OR

Modify Metadata

OR

Manage Bots

 |

-   Einstein Bots uses Translation Workbench to store translations. Turn on Translation Workbench, set up secondary languages, and define translator users in Translation Workbench. Learn more at [Add a Secondary Bot Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language_secondary.htm&language=en_US&type=5 "Create secondary languages to your existing bots.")
-   To edit translations, users must have the **Manage Translation** permission or be assigned as a translator for a specific language in Translation Workbench. Users that don’t have required permissions can only view translations in the Bot Builder.
-   Users with permissions to translate dialog text for a specific language can manage translations even with read-only access to the rest of the bot.
-   Einstein Bots supports translations entered manually, through import and export, and added by the bot.

Add translations where the end user expects to interact with the bot. Start with message and question dialog steps, and include dialog names to cover exact matching. Or you can use the included compare tool to find visible text and add translations. To learn more about how the bot processes free text from the customer’s perspective, see [Navigating Bot Conversations](https://help.salesforce.com/s/articleView?id=service.bots_service_navigating_conversations.htm&language=en_US&type=5 "To build a more efficient bot, learn about how its parts work, such as the Confused dialog, conversation repair, transfers, and intent management. Understanding the order of operation also helps you troubleshoot your bot.").

To edit the bot translations:

1.  In the Bot Builder, click **Dialogs**.
2.  Select the dialog you want to translate, and then click the **Dialog Translations** tab.
3.  From the language dropdown, select the language that you want to manage translations for.
    
    The Translations section displays the selected language’s dialog step text.
    
4.  To see another language alongside the selected language, select a language from the Compare to Language dropdown.
5.  To quickly add translations, select the dialog steps that you want to translate, and then click **Translate Selected** (beta). Or, to add translations manually, click  for the text that you want to add or edit. You can edit multiple translations in one interaction. When you’re done, save your changes.

Did this article solve your issue?

Let us know so we can improve!

YesNo