---
title: "Import Translated Articles"
source: "https://help.salesforce.com/s/articleView?id=service.knowledge_translation_import.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Import Translated Articles

Import Translated Articles[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Service](https://help.salesforce.com/s/articleView?id=service.service_cloud.htm&language=en_US&type=5)

# Import Translated Articles

If your organization sends Salesforce Knowledge articles to a vendor for translation, use the Import Article Translations feature in Setup. You can only import articles that have been exported from the same Salesforce organization. For example, you can't export articles from your test or sandbox organization and import them into your production organization.

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

1.  From Setup, enter Import Article Translations in the Quick Find box, then select **Import Article Translations**.
2.  Choose how Salesforce handles translations after they're imported.
    
    | Option | Description |
    | --- | --- |
    | Review imported translations on the Article Management tab before publishing | Add imported translations to a queue from which support reps can review them. |
    | Publish translations immediately on import | Publish imported translations without reviews. |
    
3.  Select the language of the articles you're importing.
4.  If you chose to have articles reviewed before publishing, select to send the files to a user or a queue.
5.  Click **Browse**, choose the translation .zip file to upload, and click **Open**.
    
    You must place all the translation files (meaning, those exported from Salesforce and translated by your vendor) in a folder whose name is the same as the language code. For example, put French articles in an fr folder. Zip up this folder to create your import file.
    
    Important To import translated articles successfully, verify that the file structure and their extensions match the file structure and extensions of files exported from Salesforce Knowledge for translation. For example, if the target language is French, the file structure begins as follows:
    
    ```
    import.properties
     -fr
      --articletypearticlename_kav
       ---articlename.csv
       ---[Article collateral, html, images, etc.]
    ```
    
6.  Click **Import Now**.
    
    If you have more translated articles to upload, repeat steps four through six.
    
7.  Click **Finish**.

An email notification is sent to you when your import finishes. You can view the status of your import from Setup by entering Article Imports and Exports in the Quick Find box, then selecting **Article Imports and Exports**.

#### See Also

-   [Article and Translation Import and Export Status](https://help.salesforce.com/s/articleView?id=service.knowledge_article_importer_05status.htm&language=en_US&type=5 "You can monitor the status of your article imports and exports.")
-   [Export Articles for Translation](https://help.salesforce.com/s/articleView?id=service.knowledge_translation_export.htm&language=en_US&type=5 "If your organization sends Salesforce Knowledge articles to a vendor for translation, use the Export Articles for Translation feature in Setup.")
-   [Support a Multilingual Knowledge Base](https://help.salesforce.com/s/articleView?id=service.knowledge_setup_multilingual.htm&language=en_US&type=5 "Reach a global audience by offering your knowledge base in multiple languages.")
-   [Support Knowledge Articles in Multiple Languages](https://help.salesforce.com/s/articleView?id=service.knowledge_translation_overview.htm&language=en_US&type=5 "Reach a wider audience by providing knowledge articles in any Salesforce-supported languages. Translate articles in-house or work with a localization vendor.")
-   [Salesforce Knowledge Help and Resources](https://help.salesforce.com/s/articleView?id=service.knowledge_map.htm&language=en_US&type=5 "Find the information you need about Salesforce Knowledge. Explore help documentation, developer documentation, and Trailhead modules.")

Did this article solve your issue?

Let us know so we can improve!

YesNo