---
title: "Translate Topics Names and Descriptions for Experience Cloud Sites with International Audiences"
source: "https://help.salesforce.com/s/articleView?id=experience.networks_translate_topics.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Topics Names and Descriptions for Experience Cloud Sites with International Audiences

Translate Topics Names and Descriptions for Experience Cloud Sites with International Audiences[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Translate Topics Names and Descriptions for Experience Cloud Sites with International Audiences

Use the Translation Workbench to translate topic names and descriptions in international Experience Cloud sites.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To translate topics: | 
View Setup and Configuration

AND

Be designated as a translator

 |

[](https://help.salesforce.com/s?language=en_US)

1.  From Setup, enter Translate in the Quick Find box, then select **Translate**.
2.  Select the language you’re translating into.
3.  Select **Managed Topic** for the Setup Component.
4.  For Aspect, select **Field Label** for the topic name, and **Description** for the topic description.
5.  In the Experience Name column, expand a site to see its primary topic names.
6.  To enter language-specific names for topics, double-click in the Topic Name Translation column. For descriptions, double-click in the Topic Description Translation column.
    
    Consider the following when you’re using the Translation Workbench:
    
    -   [](https://help.salesforce.com/s?language=en_US)There’s no Metadata API support for translated topic names or descriptions.
    -   [](https://help.salesforce.com/s?language=en_US)While topic name uniqueness is guaranteed in English, the translator must ensure the uniqueness of topic names in the translated language.
    -   [](https://help.salesforce.com/s?language=en_US)Modifying topic names from Experience Workspaces or Experience Management only changes the English site. All translated topic name and description changes must be made using the Translation Workbench.
    -   [](https://help.salesforce.com/s?language=en_US)If a translated topic name is entered when the site is in English mode, the translated name can appear twice in the translated site.
    -   [](https://help.salesforce.com/s?language=en_US)When topics names are translated with the Translation Workbench, hashtags in the translated sites also change. For example, #help shows as #aiuto in Italian. If the site member then reverts to English from Italian, clicking the #aiuto hashtag gives an error message rather than showing the topic detail page of #help.
    
    Note [](https://help.salesforce.com/s?language=en_US)To automatically add the translated version of a topic to translated articles, the translated topics and articles must already be uploaded in the system. Otherwise, the translated article is tagged with the English topic.
    

Did this article solve your issue?

Let us know so we can improve!

YesNo