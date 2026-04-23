---
title: "Translate Your Chat Window"
source: "https://help.salesforce.com/s/articleView?id=service.snapins_chat_localization.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Your Chat Window

Translate Your Chat Window[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Legacy Service Features](https://help.salesforce.com/s/articleView?id=service.support_legacy.htm&language=en_US&type=5)

# Translate Your Chat Window

The primary language for a chat window is set in your embedded code snippet. An extra step in Translation Workbench is required for custom labels or platform-only languages.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.legacy_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

Important

Legacy Chat will be retired on February 14, 2026. To avoid service interruptions to your end users, switch to enhanced Chat (formerly Messaging for In-App and Web). Enhanced Chat offers many of the legacy Chat [features that you love](https://help.salesforce.com/s/articleView?id=service.miaw_replacing_chat_considerations.htm&language=en_US&type=5) plus asynchronous conversations that can be picked back up at any time. Learn about migrating in [Help](https://help.salesforce.com/s/articleView?id=service.miaw_replacing_chat_considerations.htm&language=en_US&type=5) and [Trailhead](https://trailhead.salesforce.com/content/learn/modules/migrating-from-legacy-chat-to-enhanced-chat).

Set your primary language in your Embedded Service code snippet. All of your chat window labels have a default translation set for any Salesforce [fully supported or end-user language](https://help.salesforce.com/s/articleView?id=sf.faq_getstart_what_languages_does.htm&language=en_US&type=5) that you’ve added.

Follow these additional steps if you would like to create custom labels or if you want to include a platform-only language:

1.  To translate labels for your chat window, view your Embedded Service deployment in Setup.
2.  Open your Chat, Field Service or Flows settings, and click **Edit** next to Additional branding.
3.  Click the **Labels** tab to view and customize the labels in your chat window.
4.  Select the arrow next to a label and click **View Label Record**, where you can select to translate the label in the Translation Workbench.

Tip For any platform-only language, you must use custom labels and set all the labels to that language.

Important considerations for translations:

-   If no language is set in your code snippet or if it’s invalid (due to an empty string, wrong format, or language not supported), the language of the **Site Guest User** for the Site of your Embedded Service deployment is used.
-   When Translation Workbench is disabled, the language of the **Site Guest User** for the Site of your Embedded Service deployment is used.
-   To ensure that translated labels are packaged in an Embedded Service deployment, in Package Manager setup add **Language Translations** as the Component Type. Select the languages you wish to package with the deployment and click **Add to package**.
-   Not all languages are automatically available for Salesforce components. To use these end-user and platform-only languages, enable them in Languages Settings under **Company Settings**.

Tip To use translation, you must allow cookies for your browser. For example, enable “Allow third-party cookies” in Safari iOS.

#### See Also

-   [Set the Language in the Code Snippet](https://developer.salesforce.com/docs/atlas.en-us.snapins_web_dev.meta/snapins_web_dev/snapins_web_set_language.htm)
-   [Support Users in Multiple Languages](https://help.salesforce.com/s/articleView?id=sf.workbench_overview.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo