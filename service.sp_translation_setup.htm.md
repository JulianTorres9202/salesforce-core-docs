---
title: "Set Up Service Plan Translation (Optional)"
source: "https://help.salesforce.com/s/articleView?id=service.sp_translation_setup.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set Up Service Plan Translation (Optional)

Set Up Service Plan Translation (Optional)[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Set Up Service Plan Translation (Optional)

Turn on Real-Time Translations to translate service plans into service reps’ preferred language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.einstein_service_intro.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To set up Real-Time Translations for Service Assistant: | Service Planner Builder permission set. |

Note This section provides the setup steps for enabling the translation of service plans into your service reps’ preferred language. Important details and considerations are included here, but we recommend reviewing our translation reference guidance for complete details. See [Service Plan Translation](https://help.salesforce.com/s/articleView?id=service.sp_translation.htm&language=en_US&type=5 "Understand how and when translation for service plans occurs.").

By default, all service plans are drafted into your company's preferred language when the language is supported by Prompt Builder. See [Supported Languages in Prompt Builder](https://help.salesforce.com/s/articleView?id=ai.prompt_builder_localize_responses.htm&language=en_US&type=5). To have service plans translated into your service reps’ preferred language, turn on Real-Time Translations and assign them the Service Plan Translation permission set.

Service Assistant supports the same languages as Real-Time Translations. A full list of languages is provided in [Considerations for Real-Time Translations](https://help.salesforce.com/s/articleView?id=service.real_time_translations_considerations.htm&language=en_US&type=5). If a service rep’s preferred language isn’t supported, service plans always show in English.

The translation of service plans using Real-Time Translations is only available with the Agentforce for Service or Agentforce 1 licenses. If you have an Einstein for Service license and want to use Real-Time Translations, contact your Salesforce account executive.

1.  From the Service Assistant setup page, in the Case tab of the Customize Experience by Object section, go to the Turn on Real-Time Translations section.
2.  Click **Go to Real-Time Translations**.
3.  From the Real-Time Translations Setup page, under Get Started with Real-Time Translations, turn on Translate Service Plans.
4.  Assign service reps the Service Plan Translation permission set.

When Real-Time translation is enabled and service reps have the required permissions, Service Assistant automatically translates all text in a service plan into their preferred language when service reps:

-   Open a new case and a case summary is drafted.
-   Draft or redraft a service plan.
-   Open a case with an existing case summary or drafted service plan.

Considerations

-   The translation of service plans into a service rep's preferred language isn’t saved as a permanent version. Translated service plans are generated in real-time and are only visible to the service rep working the service plan. If a different service rep opens the same case, a new real-time translation occurs and the plan is shown in their preferred language. When the service rep’s preferred language isn’t supported or they don’t have the required permission set, the plan language is shown in your company's default language or English when your company language isn’t supported in Prompt Builder.
-   Translation of the name of the topic used to create the service plans that’s included in the Service Plan summary isn’t supported. The text is always shown in English. The name of the topic is shown in two places: the start of the case summary (left image above) and above the summary in a drafted service plan (see right image above).
-   If you use Real-Time Translations for Messaging and provide a custom terminology file, the file isn’t available for use in Service Assistant.
-   If you ground Service Assistant with quick actions and use custom quick actions, the names of the quick actions surfaced in the plan steps aren’t translated (1-2). The names are shown in English. To translate the names of your custom quick actions, see [Translate Metadata Labels](https://help.salesforce.com/s/articleView?id=platform.entering_translated_terms.htm&language=en_US&type=5).
-   If you ground Service Assistant in your knowledge articles, translation of the knowledge article names listed in the Sources section isn’t supported (3). The names of the knowledge articles are always shown in English. The “Sources” heading is translated. See [Knowledge Grounding](https://help.salesforce.com/s/articleView?id=service.sp_knowled_topics.htm&language=en_US&type=5).
-   If you set up the similar cases feature, the case status’ aren’t translated (4). By default, the list always shows the number and status’. The “Similar Cases” heading name is translated. See [Set Up Similar Cases](https://help.salesforce.com/s/articleView?id=service.sp_sc_ov.htm&language=en_US&type=5).

Did this article solve your issue?

Let us know so we can improve!

YesNo