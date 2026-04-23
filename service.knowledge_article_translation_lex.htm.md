---
title: "Translate Articles in Lightning Knowledge"
source: "https://help.salesforce.com/s/articleView?id=service.knowledge_article_translation_lex.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Articles in Lightning Knowledge

Translate Articles in Lightning Knowledge[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Service](https://help.salesforce.com/s/articleView?id=service.service_cloud.htm&language=en_US&type=5)

# Translate Articles in Lightning Knowledge

If your organization supports a multilingual knowledge base, give support reps and authors access to translated articles. Add authoring actions to user profiles so your support reps can access primary language versions and translation drafts.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in Lightning Experience. <a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.service_editions_reference.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To work with translated articles: | 
Manage Articles

AND

Create, Read, Edit, Delete, or Article Translation-Submit for Translation (depending on the actions assigned to the user profile)

 |

Depending on the status of your translation, and the authoring actions assigned to your user profile, you can do the following from the translation detail page.

| Action | Description | Article Status |
| --- | --- | --- |
| **Archive** | Archiving an article permanently deletes its published translations, so obsolete articles don't display to support reps and customers on your organization's Salesforce Knowledge channels. | To archive a translation, archive its primary article. |
| **Assign...** | Assigns changes to the owner of the translation | Draft translations |
| **Delete** | Deleting a translation permanently removes it from the knowledge base. You can't undelete a draft translation. | Draft translations |
| **Edit** | Editing modifies the translation's content or properties. | Draft and published translations |
| **Preview** | Previewing shows how the translation appears to end users. Voting and Chatter information isn’t available when previewing a Knowledge article. | Draft and published translations |
| **Publish...** | Publishing translations makes them visible in all channels selected. | Draft translations |
| **Submit for Translation** | Creates translation drafts for the current Primary Language Version. | \-- |

You can’t change channels on an article translation and then publish the article. Doing so generates an error.

When you change channels on an article, make sure that the channels on the article’s translations match the new channels. Also, publish translations before you publish the primary language version.

When accessing a draft article with a translation via its URL, the article defaults to your org’s primary language. If no primary language is set, the draft article is shown in the viewing user’s language, when available.

When you send a draft article out for approval, it gets locked and you cannot perform authoring actions.

To add authoring actions to a page layout created specifically for translations:

1.  Click the **Object Manager** tab and select the **Knowledge** object.
2.  Select a page layout from the **Page Layout** list. For example, a page layout that has already been created for translated articles.
3.  From **Mobile and Lightning Actions**, drag **Publish**, **Edit**, **Delete**, **Assign**, and **Submit for Translation** actions onto the page.
4.  Save your changes.

Did this article solve your issue?

Let us know so we can improve!

YesNo