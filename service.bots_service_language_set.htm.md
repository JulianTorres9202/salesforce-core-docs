---
title: "Set a Bot Conversation Language"
source: "https://help.salesforce.com/s/articleView?id=service.bots_service_language_set.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set a Bot Conversation Language

Set a Bot Conversation Language[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Set a Bot Conversation Language

You can easily define a bot conversation language at the beginning of the conversation. End users can then select their preferred language and switch to the translated text. You can also set the preferred language variable using browser information or based on a URL.

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

For bots with multiple languages, set the preferred language as early as possible in the conversation to deliver an immersive experience. You can create a variable to store the language and add a dialog to manually set it inside the conversation.

You can also write custom code to define the preferred language based on data from the source website or browser metadata. If you code to set the language in the background, include a dialog to manually change the language if the set language is incorrect.

To create a bot conversation language selection dialog:

1.  In the Bot Builder menu, select **Variables**. Click **New**.
2.  Create a variable with a Custom Type and a Text Data Type, and then save your changes.
3.  In the Bot Builder menu, select **Entities**. Click **New**.
4.  Create an entity with a Data Type of Text and Extraction Type of Value, and then save your changes.
5.  Click the name of your new entity. Set your primary language as the active language using the language dropdown.
6.  To add values, click **Add** next to Value List.
7.  Enter a value and an alternative value for each supported language. Make sure that the value matches the language code of the supported languages, as they’re the same across all languages. The alternative values, separated by commas, define ways that the language can be entered by an end user. Einstein Bots only supports translations for the languages listed in [Set or Update a Bot Primary Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language.htm&language=en_US&type=5 "Every Einstein Bot requires a primary language to be able to understand your end users. Defining a bot primary language helps with natural language processing (NLP) and named entity recognition (NER).").
8.  Change the active language to each secondary language, and provide values and alternate values.
9.  In the Bot Builder menu, select **Dialogs**. Click , and then **New Dialog**.
10.  To add a question dialog step, click  in the dialog, then select **Question**.
11.  In the Bot Asks field, ask the end user to select their preferred language. Select the custom entity and variable.
12.  In Choice Type, select Static, and include options for all available languages.
     
     Note
     
     The static options include one of the alternative values from your entity. Including multiple variations of alternative values covers cases where the end user chooses not to select the static choices and types in a value instead.
     
13.  Add a Rule Dialog Step without a condition. Select **Set Conversation Language** as the Rule Action and your custom variable as the Variable Name.
14.  Add a message dialog step with a message confirming the language has been set to the selected language.
15.  In the Next Step section, select **Start another dialog**, select the **Main Menu** dialog, and then save your changes. To enter secondary language translations, change your active language to each secondary language, and click into the Dialog Translations tab. Save your changes.

Did this article solve your issue?

Let us know so we can improve!

YesNo