---
title: "Set Up Real-Time Translations for Service Email"
source: "https://help.salesforce.com/s/articleView?id=service.email_translation_setup.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set Up Real-Time Translations for Service Email

Set Up Real-Time Translations for Service Email[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Contact Center](https://help.salesforce.com/s/articleView?id=service.support_channels.htm&language=en_US&type=5)

# Set Up Real-Time Translations for Service Email

Let service reps translate email conversations. A rep can translate an end user’s messages into the rep’s language in the case feed, as well as translate their response into the end user’s language in the email composer before sending.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:100%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a title="Learn about the Salesforce editions and user interfaces that support Email-to-Case." href="https://help.salesforce.com/s/articleView?id=service.customizesupport_email_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[](https://help.salesforce.com/s?language=en_US)

## Prepare for Real-Time Translations

Review the following checklist to ensure that you already have these elements in place.

1.  [Enable Email-to-Case](https://help.salesforce.com/s/articleView?id=service.setting_up_email-to-case.htm&language=en_US&type=5).
2.  If your org was created in Winter ‘24 or later, you already have the new Lightning Email Composer. If your org was created before then, [enable it](https://help.salesforce.com/s/articleView?id=release-notes.rn_lightning_emailcomposer_ru.htm&language=en_US&release=248&type=5).
3.  [Enable html email](https://help.salesforce.com/s/articleView?id=service.customizesupport_email_to_case_settings.htm&language=en_US&type=5).
4.  [Enable the on-demand service](https://help.salesforce.com/s/articleView?id=service.customizesupport_enabling_email_to_case.htm&language=en_US&type=5).
5.  Add a routing address.
6.  Enable Einstein setup.

[](https://help.salesforce.com/s?language=en_US)

## Prepare your Users for Real-Time Translations

Give your service reps permission to translate emails.

1.  Give your service reps the Real-Time Translations for Service Email permission set license.
2.  Give your service reps the Real-Time Translations for Service Email permission set.
3.  Give your service reps the Translate Service Emails app permission.

[](https://help.salesforce.com/s?language=en_US)

## Set Up Real-Time Translations

Turn on Real-Time Translations for Service Email and optionally upload a custom terminology file.

1.  In Setup, in the Quick Find box, enter Real-Time Translations, and select **Real-Time Translations**.
2.  Turn on **Translate Service Email**.
3.  Optionally, in the Custom Terminology section, upload a .csv, .tsx, or .tmx file with language-specific translations of any custom terms for up to 10 languages. For example, if your company name should always be Ursa Major Solar regardless of the conversation language, include it in the file. See Format Your Custom Terminology File below for more details.

Did this article solve your issue?

Let us know so we can improve!

YesNo