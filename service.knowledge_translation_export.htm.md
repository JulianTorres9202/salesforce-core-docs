---
title: "Export Articles for Translation"
source: "https://help.salesforce.com/s/articleView?id=service.knowledge_translation_export.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Export Articles for Translation

Export Articles for Translation[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Service](https://help.salesforce.com/s/articleView?id=service.service_cloud.htm&language=en_US&type=5)

# Export Articles for Translation

If your organization sends Salesforce Knowledge articles to a vendor for translation, use the Export Articles for Translation feature in Setup.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in Salesforce Classic and Lightning Experience. <a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.service_editions_reference.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To export articles: | 
Manage Salesforce Knowledge

AND

Manage Articles

AND

Manage Knowledge Article Import/Export

 |
| To view articles: | Read on the article type |
| To create articles: | Read and Create on the article type |

Place the articles to be translated in a translation queue. To enable the article export feature, create one or more queues; authors and reviewers select the queue when they submit an article for translation. Make sure that they know which queue to choose for which language.

Note You can have up to 50 exports in 24 hours and a maximum of 15 pending exports (exports that have not entered a final state such as Completed, Failed, or Canceled).

1.  Create a [translation queue](https://help.salesforce.com/s/articleView?id=service.knowledge_setup_multilingual.htm&language=en_US&type=5#knowledge_setup_multilingual "Reach a global audience by offering your knowledge base in multiple languages.") with articles for translation.
2.  On the Article Management tab, select the articles you want to translate, and click **Submit for Translation**.
3.  In the dialog box, indicate which languages to translate the articles into and assign the translations to their corresponding language translation queue.
4.  From Setup, enter Export Articles for Translation in the Quick Find box, then select **Export Articles for Translation**.
5.  Select the queue that contains the articles you're exporting.
6.  Select either:
    -   **All articles** to export every article in the queue.
    -   **Updated articles** to only export articles that have been modified or added.
7.  Click **Continue**.
8.  Select the source and target language pairs you want to export. Salesforce creates a separate .zip file for every article type in each language pair. You must retain the .zip file structure for a successful import.
9.  To have the files reviewed or published after being translated, select a user or a queue.
10.  Select the file character encoding.
     
     -   ISO-8859-1 (General US & Western European, ISO-LATIN-1)
     -   Unicode
     -   Unicode (UTF-8) _default_
     -   Japanese (Windows)
     -   Japanese (Shift\_JIIS)
     -   Chinese National Standard (GB18030)
     -   Chinese Simplified (GB2312)
     -   Chinese Traditional (Big5)
     -   Korean
     -   Unicode (UTF-16, Big Endian)
     
11.  Select the delimiter for the .csv files. The delimiter is the separator for columns when the file is converted to table form. Your options are tab (default) or comma.
12.  Click **Export Now**.

You’re notified by email when your export is complete. You can also check the status of your export by viewing the Article Import and Export Queue. From Setup, enter Article Imports and Exports in the Quick Find box, then select **Article Imports and Exports**.

Unzip the exported files, but retain the file structure for a successful import.

#### See Also

-   [Import Translated Articles](https://help.salesforce.com/s/articleView?id=service.knowledge_translation_import.htm&language=en_US&type=5 "If your organization sends Salesforce Knowledge articles to a vendor for translation, use the Import Article Translations feature in Setup. You can only import articles that have been exported from the same Salesforce organization. For example, you can't export articles from your test or sandbox organization and import them into your production organization.")
-   [Support a Multilingual Knowledge Base](https://help.salesforce.com/s/articleView?id=service.knowledge_setup_multilingual.htm&language=en_US&type=5 "Reach a global audience by offering your knowledge base in multiple languages.")
-   [Support Knowledge Articles in Multiple Languages](https://help.salesforce.com/s/articleView?id=service.knowledge_translation_overview.htm&language=en_US&type=5 "Reach a wider audience by providing knowledge articles in any Salesforce-supported languages. Translate articles in-house or work with a localization vendor.")
-   [Salesforce Knowledge Help and Resources](https://help.salesforce.com/s/articleView?id=service.knowledge_map.htm&language=en_US&type=5 "Find the information you need about Salesforce Knowledge. Explore help documentation, developer documentation, and Trailhead modules.")

Did this article solve your issue?

Let us know so we can improve!

YesNo