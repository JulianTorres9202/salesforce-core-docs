---
title: "Add or Remove a Secondary Bot Language"
source: "https://help.salesforce.com/s/articleView?id=service.bots_service_language_secondary.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Add or Remove a Secondary Bot Language

Add or Remove a Secondary Bot Language[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Add or Remove a Secondary Bot Language

Create secondary languages to your existing bots.

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

-   To add a secondary language to an Einstein Bot, it needs a primary language set. Before a language appears as an available secondary language for a bot, the language must be enabled in Language Settings and activated in Translation Workbench.
-   To test a single-language bot with secondary languages, we recommend that you clone the bot first before adding secondary languages. Read more at [Clone a Bot](https://help.salesforce.com/s/articleView?id=service.bots_service_clone.htm&language=en_US&type=5 "Admins can clone a bot quickly to help with development, or they can create a similar bot for a different use case.").
-   Einstein Bots only supports languages listed at [Define Languages for your Einstein Bot](https://help.salesforce.com/s/articleView?id=service.bots_service_language_define.htm&language=en_US&type=5 "Your global customers expect your bots to understand their native language. To know what your customers are saying, your bots must know how a language works. Bots use natural language understanding (NLU) and named entity recognition (NER) to understand language and local details such as dates, currency, or number formatting. Einstein Bots that use a specific language can better understand the customer and route them to the correct dialog."). To get access to all of the languages Einstein Bots supports, review [Salesforce supported languages](https://help.salesforce.com/s/articleView?id=xcloud.faq_getstart_what_languages_does.htm&language=en_US&type=5). Where necessary, [enable end-user and platform-only languages](https://help.salesforce.com/s/articleView?id=xcloud.admin_select_languages_for_your_org.htm&language=en_US&type=5) on the Language Settings page in Setup. Language support varies by intent model.
-   Translation Workbench Prerequisites
    -   Einstein Bots uses Translation Workbench to store translations. Turn on Translation Workbench, set up secondary languages, and define translator users in Translation Workbench before moving to the Bot Builder.
    -   To edit translations, users require the **Manage Translation** permission or assignment as a translator for a specific language in Translation Workbench. Users without the correct permissions can view but not edit translations in the Bot Builder.
    -   Users with permissions to translate dialog text for a specific language can manage translations even with read-only access to the rest of the bot.
    -   Einstein Bots supports translations entered manually or through import and export. When you import and export translations, the dialog name field must be complete for each dialog and language in order to populate the translated messages inside of the dialog.

1.  In the Bot Builder menu, click **Overview**.
2.  In Conversation Languages, click **Add**.
3.  Select the secondary language from the dropdown, and click **Add**.

To remove a secondary bot language, click **Remove** from the dropdown next to the language on the Bot Overview page. Removing a secondary language removes it from the bot. Your translated content and utterances reappear if you add the language back.

Did this article solve your issue?

Let us know so we can improve!

YesNo