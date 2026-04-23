---
title: "Define Languages for Your Einstein Bot"
source: "https://help.salesforce.com/s/articleView?id=service.bots_service_language_define.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Define Languages for Your Einstein Bot

Define Languages for Your Einstein Bot[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Define Languages for Your Einstein Bot

Your global customers expect your bots to understand their native language. To know what your customers are saying, your bots must know how a language works. Bots use natural language understanding (NLU) and named entity recognition (NER) to understand language and local details such as dates, currency, or number formatting. Einstein Bots that use a specific language can better understand the customer and route them to the correct dialog.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.einstein_service_intro.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

You can build Einstein Bots for one language or multiple languages. You must define at least one primary language for each Einstein Bot on the Bot Overview page. See [Set or Update a Bot Primary Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language.htm&language=en_US&type=5 "Every Einstein Bot requires a primary language to be able to understand your end users. Defining a bot primary language helps with natural language processing (NLP) and named entity recognition (NER).") and [Add or Remove a Secondary Bot Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language_secondary.htm&language=en_US&type=5 "Create secondary languages to your existing bots.").

To view and edit language-specific data in the Bot Builder, you must enable the language in Language Settings, activate it in Translation Workbench, and add it to Conversation Languages on the Bot Overview page. Then you can add or edit dialog translations on the Dialog Translations tab. To quickly translate a dialog to a different language, select dialog steps, and then click **Translate Selected**.

Multi-language bots share dialog logic and deliver dialog translations to your end user. To show language choices at the beginning of the conversation so the end user can select their conversation language, create a question dialog step that offers each language as a static choice. See [Set a Bot Conversation Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language_set.htm&language=en_US&type=5 "You can easily define a bot conversation language at the beginning of the conversation. End users can then select their preferred language and switch to the translated text. You can also set the preferred language variable using browser information or based on a URL.").

To ensure that a bot respects rule conditions in multiple languages, on Rule dialog steps, use the OR condition requirements to specify text value conditions in each language.

Multi-language bots have one F1 score on the Model Management page. You can download the data and filter metrics by language.

In multi-language bots, dialogs assigned to the Bot Options Menu only show in the primary language.

Some bot templates and blocks support multiple languages. For more details on language support for a system template, see [Explore Einstein Bot System Templates](https://help.salesforce.com/s/articleView?id=service.bots_service_template_directory.htm&language=en_US&type=5 "Learn about bot templates designed for specific clouds and use cases.").

## Supported Languages

Einstein Bots supports right-to-left languages in the Bot Builder based on the language you specify in your personal settings.

To access all of the languages that Einstein Bots supports, see [Salesforce supported languages](https://help.salesforce.com/s/articleView?id=xcloud.faq_getstart_what_languages_does.htm&language=en_US&type=5). Where necessary, [enable end-user and platform-only languages](https://help.salesforce.com/s/articleView?id=xcloud.admin_select_languages_for_your_org.htm&language=en_US&type=5) on the Language Settings page in Setup.

Languages that are supported by the original intent model must have at least 20 or 50 utterances per intent.

For some languages, named entity recognition (NER) is partially supported only for phone number and currency.

-   Phone numbers are recognized only when numbers are written in Arabic numerals (0-9).
-   Currency is recognized only when the currency code is written in English letters (A-Z) and the numbers are written in Arabic numerals (0-9). Some languages recognize English currency names with or without the currency code (dinar, euro, rial, riyal, rupee).

| Language | Intent Model Support | NER Support | Beta Service |
| --- | --- | --- | --- |
| 
Arabic

(supported in the Bot Builder and Enhanced Chat channels only)

 | Cross-Lingual | Full support for date, time, currency, number, and phone number. |  |
| Bangla / Bengali | Cross-Lingual | Full support for date, time, currency, and number. |  |
| Bulgarian | Cross-Lingual | Full support for date, time, currency, and number. |  |
| Catalan | Cross-Lingual | Full support for date, time, currency, and number. |  |
| Chinese (Simplified) | 

-   Cross-Lingual
-   Original

 |  |   |
| Chinese (Traditional) | 

-   Cross-Lingual
-   Original

 |  |   |
| Croatian | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency and phone number.

 |   |
| Czech | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency.

 |  |
| Danish | 

-   Cross-Lingual
-   Original

 |  |   |
| Dutch | 

-   Cross-Lingual
-   Original

 |  |   |
| English | 

-   Cross-Lingual
-   Original

 |  |   |
| English (UK) | 

-   Cross-Lingual
-   Original

 |  |   |
| Estonian | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency.

 |  |
| Finnish | Cross-Lingual | 

-   Full support for number.
-   Partial support for date, time, currency, and phone number.

 |  |
| French | 

-   Cross-Lingual
-   Original

 |  |   |
| Georgian | Cross-Lingual | Full support for date, time, currency, and number. |  |
| German | 

-   Cross-Lingual
-   Original

 | [](https://help.salesforce.com/s?language=en_US)

-   Full support for time, currency, and number.
    
-   Partial support for date.

 |   |
| Greek | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency and phone number.

 |   |
| 

Hebrew

(supported in the Bot Builder and Enhanced Chat channels only)

 | Cross-Lingual | Full support for date, time, currency, and number. |   |
| Hindi | Cross-Lingual | 

-   Full support for date, time, and phone number.
-   Partial support for currency, and number.

 |   |
| Irish | Cross-Lingual | Full support for date, time, currency, and number. |  |
| Italian | 

-   Cross-Lingual
-   Original

 | 

-   Full support for time, currency, and number.
-   Partial support for date.

 |   |
| Japanese | 

-   Cross-Lingual
-   Original

 |  |   |
| Korean | 

-   Cross-Lingual
-   Original

 |  |   |
| Latvian | Cross-Lingual | 

-   Full support for time and phone number.
-   Partial support for date, number, and currency.

 |  |
| Lithuanian | Cross-Lingual | 

-   Full support for time and phone number.
-   Partial support for date, number, and currency.

 |  |
| Malayalam | Cross-Lingual | Full support for date, time, and number. |  |
| Norwegian | Cross-Lingual | 

-   Full support for time and phone number.
-   Partial support for date, number, and currency.

 |  |
| Polish | Cross-Lingual | 

-   Full support for date, time, and phone number.
-   Partial support for number and currency.

 |   |
| Portuguese (Brazil) | 

-   Cross-Lingual
-   Original

 |  |   |
| Portuguese (Europe) | 

-   Cross-Lingual
-   Original

 |  |   |
| Romanian | Cross-Lingual | 

Full support for date, time, currency, and number.

 |   |
| Russian | 

-   Cross Lingual
-   Original

 |  |   |
| Slovak | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency.

 |  |
| Spanish | 

-   Cross-Lingual
-   Original

 |  |   |
| Spanish (Mexico) | 

-   Cross-Lingual
-   Original

 |  |   |
| Swedish | 

-   Cross-Lingual
-   Original

 |  |   |
| Tagalog | Cross-Lingual | 

-   Full support for date, time, and phone number.
-   Partial support for number.

 |  |
| Tamil | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency.

 |  |
| Telugu | Cross-Lingual | Full support for date, time, and number. |  |
| Thai | Cross-Lingual | 

-   Full support for number and phone number.
-   Partial support for date, time, and currency.

 |  |
| Turkish | Cross-Lingual | 

-   Full support for date, time, and phone number.
-   Partial support for number and currency.

 |  |
| Ukrainian | Cross-Lingual | 

-   Full support for date, time, and number.
-   Partial support for currency.

 |  |
| Vietnamese | Cross-Lingual |  |   |

Support for some languages in Einstein Bots is a Beta Service. Customer may opt to try such Beta Service in its sole discretion. Any use of the Beta Service is subject to the applicable Beta Services Terms provided at [Agreements and Terms](https://www.salesforce.com/company/legal/agreements/).

-   **[Set or Update a Bot Primary Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language.htm&language=en_US&type=5)**  
    Every Einstein Bot requires a primary language to be able to understand your end users. Defining a bot primary language helps with natural language processing (NLP) and named entity recognition (NER).
-   **[Add or Remove a Secondary Bot Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language_secondary.htm&language=en_US&type=5)**  
    Create secondary languages to your existing bots.
-   **[Manage Secondary Language Translations](https://help.salesforce.com/s/articleView?id=service.bots_service_language_translations.htm&language=en_US&type=5)**  
    Edit bot translations directly in each bot dialog.
-   **[Set a Bot Conversation Language](https://help.salesforce.com/s/articleView?id=service.bots_service_language_set.htm&language=en_US&type=5)**  
    You can easily define a bot conversation language at the beginning of the conversation. End users can then select their preferred language and switch to the translated text. You can also set the preferred language variable using browser information or based on a URL.

Did this article solve your issue?

Let us know so we can improve!

YesNo