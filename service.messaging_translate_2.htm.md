---
title: "Set Up Real-Time Translations"
source: "https://help.salesforce.com/s/articleView?id=service.messaging_translate_2.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set Up Real-Time Translations

Set Up Real-Time Translations[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Contact Center](https://help.salesforce.com/s/articleView?id=service.support_channels.htm&language=en_US&type=5)

# Set Up Real-Time Translations

Allow service reps and customers to communicate in different languages. When an end user messages your business, Real-Time Translations converts the message into the service rep’s preferred language. The rep can type their response in their own preferred language, and have it translated to the end user’s language before sending. Supervisors can also use Real-Time Translations when monitoring active conversations.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="2" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.messaging_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions.</a></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a name="messaging_translate_2__image_lkc_rgf_5cc" lwc-3eigj2skqo3="" href="https://help.salesforce.com/s?language=en_US"></a><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="Checkmark" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/checkmark.png" id="messaging_translate_2__image_lkc_rgf_5cc" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article applies to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Enhanced In-App Chat, Enhanced Web Chat, Enhanced WhatsApp, Enhanced Facebook Messenger, Enhanced SMS, Enhanced Apple Messages for Business, Enhanced LINE, and Bring Your Own Channel</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="X icon" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/crossmark.png" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article doesn’t apply to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Standard Facebook Messenger and Standard SMS channels</td></tr></tbody></table>

| User Permissions |
| --- |
| To view and send translated messages: | 
Real-Time Translations permission set license

AND

Translate Enhanced Conversations

 |

[](https://help.salesforce.com/s?language=en_US)

## Prepare your Org for Real-Time Translations

Add the Agentforce for Service SKU.

[](https://help.salesforce.com/s?language=en_US)

## Prepare your Users for Real-Time Translations

Add and configure permissions for a successful translation experience.

1.  In Setup, enter **Users** in the Quick Find box and select Users.
2.  Click on a user record.
3.  Under Permission Set License Assignments, find and select **Real-Time Translations**.
4.  Add the Translate Enhanced Conversations app permission to a new or existing permission set.
5.  Assign the permission set to your user.
6.  Repeat these steps for each user who’ll use translations.

[](https://help.salesforce.com/s?language=en_US)

## Set Up Real-Time Translations

Turn on, customize, and test Real-Time Translations

1.  In Setup, enter Real-Time Translations in the Quick Find box and select **Real-Time Translations**.
2.  Turn on Real-Time Translations for Enhanced Chat and Enhanced Messaging.
3.  Optionally, in the Custom Terminology section, upload a .csv, .tsx, or .tmx file with language-specific translations of any custom terms for up to 10 languages. For example, if your company name should always be Ursa Major Solar regardless of the conversation language, include it in the file. See Format Your Custom Terminology File below for more details.
4.  To test the feature, select a language to translate from and another to translate to. Then enter a message into the Text field.
5.  To be transparent, let customers know that reps might use a machine translation tool when chatting with them. You can do this by customizing the Start Conversation auto-response (all channels) or your chat window header or Terms and Conditions (Enhanced Chat only).

[](https://help.salesforce.com/s?language=en_US)

## Format Your Custom Terminology File

Configure how your brand's terminology appears in your supported languages. Then upload it as a .csv, .tsx, or .tmx file. Custom terminology is multi-directional, meaning that both service reps and end users see the terms that you provide. Review best practices and limitations for uploading a custom terminology file.

#### See Also

-   [_Salesforce Help:_ Translate a Messaging Conversation](https://help.salesforce.com/s/articleView?id=service.service_rep_translate.htm&language=en_US&type=5 "Real-Time Translations lets service reps and customers communicate in their preferred language.")

Did this article solve your issue?

Let us know so we can improve!

YesNo