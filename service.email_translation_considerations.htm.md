---
title: "Considerations and Limitations for Real-Time Translations on Service Email"
source: "https://help.salesforce.com/s/articleView?id=service.email_translation_considerations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Considerations and Limitations for Real-Time Translations on Service Email

Considerations and Limitations for Real-Time Translations on Service Email[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Contact Center](https://help.salesforce.com/s/articleView?id=service.support_channels.htm&language=en_US&type=5)

# Considerations and Limitations for Real-Time Translations on Service Email

Before starting your setup process, review the considerations and limitations for Real-Time Translations for Service Email. Note that considerations and supported languages vary between target and source languages, and between case feed and email composer.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:100%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a title="Learn about the Salesforce editions and user interfaces that support Email-to-Case." href="https://help.salesforce.com/s/articleView?id=service.customizesupport_email_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[](https://help.salesforce.com/s?language=en_US)

## General Considerations

These considerations are shared between translating emails in the case feed and translating replies in the email composer.

-   Translation doesn’t work on email in the Salesforce mobile app. It only works on a desktop browser.
-   Translation only supports an email body that’s encoded in UTF-8.
-   We can translate up to 10 kilobytes of email text at a time. If the text exceeds this size limit, the email isn’t translated.
-   Translation doesn’t consider the Locale field on the user profile.
-   Any formatting such as fonts, tables, or images is lost during the translation process. Formatting must be added to the text after translation.

[](https://help.salesforce.com/s?language=en_US)

## Considerations for Translating Emails in the Case Feed

These considerations are specific to the experience of translating inbound email text in the case feed.

-   The Target language is the service rep’s language and the Source language is the language detected in the email that was received. Typically, this is the end user’s language. It could also be the language of a different service rep who responded in the email thread.
-   The rep can set their preferred language (or the Target language) by clicking their user avatar and selecting **Settings**. After selecting **Language & Time Zones**, the rep can set the **Language** drop-down field. See a list of supported languages below.
-   We only translate the content above the quoted previous email content. We attempt to detect quotation lines, but if unable to do so, more content could be translated.
-   We show a disclaimer at the end of the translated email body, above detected quotation lines to indicate that it was translated. This disclaimer is subject to the supported languages for Service reps in case feed. See a list of supported languages below.

[](https://help.salesforce.com/s?language=en_US)

## Considerations for Translating in the Email Composer

These considerations are specific to the experience of translating an email reply in the email composer.

-   In email composer translations, the Target language is the language of the email being replied to. This is most likely the end user’s language. However, if the previous email was from a different service rep, the Target language is the service rep’s language. When we detect the language of previous email, we only look at the content above quoted email content. This ensures the language is associated with the author of the most recent email, not the other authors in prior emails.
-   In email composer translations, the Source language is the selected content to translate. In most cases, this is the service rep’s language.
-   We add a disclaimer that the email has been translated. The disclaimer appears in the end user’s language. If the end user’s language is unsupported, the disclaimer appears in English. See supported languages below.
-   Formatting, such as tables, images, or mixed fonts, aren't preserved in translation. Instead of selecting a whole table, select content in a cell of the table.
-   If [Reply with new content only](https://help.salesforce.com/s/articleView?id=service.customizesupport_email_to_case_settings.htm&language=en_US&type=5) is off, we recommend writing new content above the quoted previous email. Then, select the content that you want to translate above the quoted previous email content. To translate the quotation lines (including replied, forward indication, or date), we recommend selecting individual words to translate.
-   If [Reply with new content only](https://help.salesforce.com/s/articleView?id=service.customizesupport_email_to_case_settings.htm&language=en_US&type=5) is on, we recommend keeping the threading token, and not adding new content below it. If the threading token is not automatically inserted, we recommend adding new content from the top.
-   To preserve the language of the previous email for translation, don’t delete the content of the email body, either manually or by selecting Clear email and revert.

[](https://help.salesforce.com/s?language=en_US)

## Supported Languages

Real-Time Translations supports different sets of languages for Source (input) language and Target (output) language. The sender of the Source and Target languages depends on whether translation occurs in the case feed or the email composer. Here’s a breakdown:

Case Feed

-   Source language: The end user’s language.
-   Target language: The service rep’s language. See Considerations for Translating Emails in the Case Feed for instructions on how to set this language.

Email Composer

-   Source Language: The selected content to translate. Typically, this is the service rep’s language.
-   Target language: The language of the email being replied to. Typically, this is the end user’s language.

Supported Source Languages for Case Feed

Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Bengali, Bosnian, Bulgarian, Catalan, Chinese (Simplified), Chinese (Traditional), Croatian, Czech, Danish, Dari, Dutch, English, Estonian, Farsi (Persian), Filipino (Tagalog), Finnish, French, French (Canada), Georgian, German, Greek, Gujarati, Haitian Creole, Hausa, Hebrew, Hindi, Hungarian, Icelandic, Indonesian, Irish, Italian, Japanese, Kannada, Kazakh, Korean, Latvian, Lithuanian, Macedonian, Malay, Malayalam, Maltese, Marathi, Mongolian, Norwegian (Bokmål), Pashto, Polish, Portuguese (Brazil), Portuguese (Portugal), Punjabi, Romanian, Russian, Serbian, Sinhala, Slovak, Slovenian, Somali, Spanish, Spanish (Mexico), Swahili, Swedish, Tamil, Telugu, Thai, Turkish, Ukrainian, Urdu, Uzbek, Vietnamese, Welsh

Supported Target Languages for Case Feed

Arabic, Bulgarian, Catalan, Chinese (Traditional), Chinese (Simplified), Croatian, Czech, Danish, Dutch, English, English (UK), Finnish, French, German, Greek, Hebrew, Hungarian, Italian, Indonesian, Japanese, Korean, Norwegian, Polish, Portuguese (Brazil), Portuguese (Portugal), Romanian, Russian, Slovene, Slovak, Spanish, Spanish (Mexico), Swedish, Thai, Turkish, Ukrainian, Vietnamese

Supported Source and Target Languages for Email Composer

Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Bengali, Bosnian, Bulgarian, Catalan, Chinese (Simplified), Chinese (Traditional), Croatian, Czech, Danish, Dari, Dutch, English, Estonian, Farsi (Persian), Filipino (Tagalog), Finnish, French, French (Canada), Georgian, German, Greek, Gujarati, Haitian Creole, Hausa, Hebrew, Hindi, Hungarian, Icelandic, Indonesian, Irish, Italian, Japanese, Kannada, Kazakh, Korean, Latvian, Lithuanian, Macedonian, Malay, Malayalam, Maltese, Marathi, Mongolian, Norwegian (Bokmål), Pashto, Polish, Portuguese (Brazil), Portuguese (Portugal), Punjabi, Romanian, Russian, Serbian, Sinhala, Slovak, Slovenian, Somali, Spanish, Spanish (Mexico), Swahili, Swedish, Tamil, Telugu, Thai, Turkish, Ukrainian, Urdu, Uzbek, Vietnamese, Welsh

Supported Languages for Custom Terminology File

Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Bengali, Bosnian, Bulgarian, Catalan, Chinese (Simplified), Chinese (Traditional), Croatian, Czech, Danish, Dari, Dutch, English, Estonian, Farsi (Persian), Filipino (Tagalog), Finnish, French, French (Canada), Georgian, German, Greek, Gujarati, Haitian Creole, Hausa, Hebrew, Hindi, Hungarian, Icelandic, Indonesian, Irish, Italian, Japanese, Kannada, Kazakh, Korean, Latvian, Lithuanian, Macedonian, Malay, Malayalam, Maltese, Marathi, Mongolian, Norwegian (Bokmål), Pashto, Polish, Portuguese (Brazil), Portuguese (Portugal), Punjabi, Romanian, Russian, Serbian, Sinhala, Slovak, Slovenian, Somali, Spanish, Spanish (Mexico), Swahili, Swedish, Tamil, Telugu, Thai, Turkish, Ukrainian, Urdu, Uzbek, Vietnamese, Welsh

Supported Languages for Translation Disclaimer for Case Feed and Email Composer

Arabic, Bulgarian, Catalan, Chinese (Traditional), Chinese (Simplified), Croatian, Czech, Danish, Dutch, English, English (UK), Finnish, French, German, Greek, Hebrew, Hungarian, Italian, Indonesian, Japanese, Korean, Norwegian, Polish, Portuguese (Brazil), Portuguese (Portugal), Romanian, Russian, Slovene, Slovak, Spanish, Spanish (Mexico), Swedish, Thai, Turkish, Ukrainian, Vietnamese

[](https://help.salesforce.com/s?language=en_US)

## Usage Types for Real-Time Translations

These considerations are specific to the experience of translating an email reply in the email composer.

| Digital Wallet Card | usage type | Description | notes |
| --- | --- | --- | --- |
| Flex Credits | Translation | 
Translation converts text from one human language into text of another, a process executed by machine translation models. Translation usage is metered by the number of characters processed for the translation.

To understand how your consumption appears in the Digital Wallet, consider a scenario where you process 9,000 characters for translation. Because this usage is in units of one million characters, your actual consumption is 0.009 units (9,000 divided by 1,000,000). In the Digital wallet, this usage is rounded to two decimal places and the value is displayed as 0.01 units.

 | 

Translation usage includes a monthly allocation of 250,000 characters per user for every Agentforce add-on license.

This limit refreshes monthly, and any unused characters do not roll over to the next month.

When the 250,000 character limit is exceeded within a month, any further usage will automatically draw down Flex Credits.

 |

[](https://help.salesforce.com/s?language=en_US)

## Custom Terminology File Limits and Considerations

Follow these best practices when formatting your custom terminology file.

-   Your file should be UTF-8 encoded.
-   When you format your file, keep it uncluttered. Only include terms that you want translated or preserved in a particular way.
-   The terminology file is case-sensitive. If you want both the capitalized and non-capitalized versions of a word translated, include an entry for each version.
-   Special characters and formatting don’t always translate into another language. Avoid these if possible.

We also recommend reviewing limitations before preparing your custom terminology file.

-   Your custom terminology file is considered at translation, but it’s not guaranteed that the translation service will implement it accurately.
-   You can upload one custom terminology file at a time. A new upload replaces the former upload.
-   The maximum custom terminology file size is 10 MB.
-   The maximum number of target languages per custom terminology file is 10.
-   The maximum source and target text length per custom terminology term is 200 bytes.

We also offer examples of formatting .csv or .tmx file types.

| File TYpe | Example |
| --- | --- |
| 
CSV (comma separated values)

 | 

```
en,es,fr,it
Ursa Major Solar,Ursa Major Solar,Ursa Major Solar,Ursa Major Solar
```

 |
| 

TMX (Translation Memory eXchange)

 | 

```
<?xml version="1.0" encoding="UTF-8"?>
 <tmx version="1.4">
  <header
     creationtool="XYZTool" creationtoolversion="0"
     datatype="PlainText" segtype="sentence"
     adminlang="en-us" srclang="en"
     o-tmf="test"/>
  <body>
    <tu>
      <tuv xml:lang="en">
        <seg>Amazon Photos</seg>
      </tuv>
      <tuv xml:lang="fr">
        <seg>Amazon Photos</seg>
      </tuv>
      <tuv xml:lang="es">
        <seg>Amazon Photos</seg>
      </tuv>
    </tu>   
  </body>
 </tmx>
```

 |

Did this article solve your issue?

Let us know so we can improve!

YesNo