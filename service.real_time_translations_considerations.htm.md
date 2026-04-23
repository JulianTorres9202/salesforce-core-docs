---
title: "Considerations and Limitations for Real-Time Translations for Enhanced Chat and Enhanced Messaging"
source: "https://help.salesforce.com/s/articleView?id=service.real_time_translations_considerations.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Considerations and Limitations for Real-Time Translations for Enhanced Chat and Enhanced Messaging

Considerations and Limitations for Real-Time Translations for Enhanced Chat and Enhanced Messaging[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Contact Center](https://help.salesforce.com/s/articleView?id=service.support_channels.htm&language=en_US&type=5)

# Considerations and Limitations for Real-Time Translations for Enhanced Chat and Enhanced Messaging

Before starting your setup process, review the considerations and limitations for Real-Time Translations for Enhanced Chat and Enhanced Messaging.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="2" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.messaging_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions.</a></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a name="real_time_translations_considerations__d556e2463" lwc-3eigj2skqo3="" href="https://help.salesforce.com/s?language=en_US"></a><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="Checkmark" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/checkmark.png" id="real_time_translations_considerations__d556e2463" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article applies to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Enhanced In-App Chat, Enhanced Web Chat v1, Enhanced Web Chat v2, Enhanced WhatsApp, Enhanced Facebook Messenger, Enhanced SMS, Enhanced Apple Messages for Business, and Enhanced LINE channels</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="X icon" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/crossmark.png" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article doesn’t apply to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Standard Facebook Messenger, Standard SMS, and Bring Your Own Channel</td></tr></tbody></table>

## General Considerations

-   The [Agentforce for Service](https://help.salesforce.com/s/articleView?id=service.einstein_service_intro.htm&language=en_US&type=5) add-on is required to enable and use Real-Time Translations.
-   Salesforce uses the customer's three most recent messages to detect their preferred language. Service reps’ language preferences are set in their user profile.
-   If the customer and the service rep use the same language, no translation option is displayed to the rep.
-   If language detection is incorrect, wait a couple of messages and refresh to try language detection again.

## Supported Languages

Supported languages include: Afrikaans, Albanian, Amharic, Arabic, Armenian, Azerbaijani, Bengali, Bosnian, Bulgarian, Catalan, Chinese (Simplified), Chinese (Traditional), Croatian, Czech, Danish, Dari, Dutch, English, Estonian, Farsi (Persian), Filipino (Tagalog), Finnish, French, French (Canada), Georgian, German, Greek, Gujarati, Haitian Creole, Hausa, Hebrew, Hindi, Hungarian, Icelandic, Indonesian, Irish, Italian, Japanese, Kannada, Kazakh, Korean, Latvian, Lithuanian, Macedonian, Malay, Malayalam, Maltese, Marathi, Mongolian, Norwegian (Bokmål), Pashto, Polish, Portuguese (Brazil), Portuguese (Portugal), Punjabi, Romanian, Russian, Serbian, Sinhala, Slovak, Slovenian, Somali, Spanish, Spanish (Mexico), Swahili, Swedish, Tamil, Telugu, Thai, Turkish, Ukrainian, Urdu, Uzbek, Vietnamese, and Welsh.

## Usage Types for Real-Time Translations

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

## Custom Terminology File Limits and Considerations

Follow these best practices when formatting your custom terminology doc.

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