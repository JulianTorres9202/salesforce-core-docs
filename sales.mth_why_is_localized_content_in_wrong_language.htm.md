---
title: "Troubleshoot Localized Content That Appears in the Wrong Language"
source: "https://help.salesforce.com/s/articleView?id=sales.mth_why_is_localized_content_in_wrong_language.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Troubleshoot Localized Content That Appears in the Wrong Language

Troubleshoot Localized Content That Appears in the Wrong Language[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Enablement Sites (myTrailhead)](https://help.salesforce.com/s/articleView?id=sales.mth_intro.htm&language=en_US&type=5)

# Troubleshoot Localized Content That Appears in the Wrong Language

Did you localize enablement site content for a particular language and a user selected that language, but the content still appears in the source language? Most likely, the number of units in a module differs between the source and localized files. When content isn’t available for a selected language, an enablement site falls back to the source language. To resolve this issue, work with your localization team or vendor to correct the number of units in a module in the localized files.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</td></tr></tbody></table>

| User Roles and Permissions |
| --- |
| **Enablement Site User Roles** |   |
| This topic supports these enablement site roles: | 
-   Release Managers
-   Localization Team or Vendor

 |
| **Required System Permissions** |   |
| To create and edit content with Trailmaker Content: | Create Content |
| To upload content from Trailmaker Content to Trailmaker Release: | 

Create Content

AND

Manage Releases

 |
| To create and manage releases with Trailmaker Release: | Manage Releases |
| To view the full release preview: | Preview Release |

1.  Find the backpack for the content that you want to change. You can:
    
    -   Access the backpack in your company’s version control system.
    -   Download the latest released version of the backpack from Trailmaker Release. To learn more, see [Download a Backpack from Trailmaker Release](https://help.salesforce.com/s/articleView?id=sales.mth_tm_release_download.htm&language=en_US&type=5 "From Trailmaker Release, you can download the backpack ZIP file for a module or trail published in your company’s enablement site. With this backpack, your content creators can easily access the latest released version of content the next time they want to update it.").
    
2.  Import the backpack into Trailmaker Content by completing the steps in [Import a Backpack into Trailmaker Content](https://help.salesforce.com/s/articleView?id=sales.mth_upload_published_or_archived_content_to_tm_content.htm&language=en_US&type=5 "You can add learning content into your workspace from a backpack ZIP file that you saved or downloaded. This workflow is helpful when you want to collaborate on content that other content creators started in their own workspace. Or, follow these steps when you want to update published content or restore archived content. You can also import a content template that you downloaded.").
3.  Make your structural changes to the source content. For example, add a unit to the module.
4.  Send the backpack with the new unit to your localization team or vendor. Your vendor makes the necessary changes to the translated files.
5.  When the localization vendor returns the revised module, ensure that the backpack structure is correct by reviewing the [guidelines for localizing files in a backpack](https://help.salesforce.com/s/articleView?id=sales.mth_localize_files.htm&language=en_US&type=5 "Your localization team or vendor can localize only certain trail, module, unit, and quiz information in your backpack’s files.").
6.  In Trailmaker Content, add the content to an unpublished release by completing the steps in [Add Content to a Release from Trailmaker Content](https://help.salesforce.com/s/articleView?id=sales.mth_add_content_to_release_from_tm_content.htm&language=en_US&type=5 "After you create your module and quizzes and assign all the necessary metadata, add the content to a release.").
7.  In Trailmaker Release, preview and publish the release by completing the steps in [Preview a Release in Trailmaker Release](https://help.salesforce.com/s/articleView?id=sales.mth_preview_content_on_mytrailhead.htm&language=en_US&type=5 "Your content stakeholders can preview all the new or changed trails and modules that you plan to publish in a release. The full release preview shows new or changed content in the context of all published content in your company’s enablement site. Only users with the appropriate permission can access the full release preview.") and [Publish Content with Trailmaker Release](https://help.salesforce.com/s/articleView?id=sales.mth_publish_content_with_tm_release.htm&language=en_US&type=5 "After you test, proofread, and validate your content, you can publish the release's new or changed content to your enablement site.").

#### See Also

-   [Translate Enablement Site Content to Other Languages](https://help.salesforce.com/s/articleView?id=sales.mth_localize_your_content.htm&language=en_US&type=5 "Learners can select a different language for viewing your enablement site. To provide localized versions of your learning content for supported languages, work with a localization team or vendor.")
-   [Give Content Files to a Localization Team or Vendor](https://help.salesforce.com/s/articleView?id=sales.mth_give_files_to_localization_vendor.htm&language=en_US&type=5 "To add localized content, send the backpack to your localization team or vendor. The backpack is a ZIP file, downloaded from Trailmaker, that contains the module or trail’s source files. You can send the backpack ZIP file or give the vendor access to your version control system (VCS) to download the backpack. After the vendor translates your content, the vendor can upload the backpack—updated with the localized files—to your VCS. Then, you can publish the localized content.")
-   [Guidelines for Localizing Files in a Backpack](https://help.salesforce.com/s/articleView?id=sales.mth_localize_files.htm&language=en_US&type=5 "Your localization team or vendor can localize only certain trail, module, unit, and quiz information in your backpack’s files.")
-   [Preview and Publish Localized Content](https://help.salesforce.com/s/articleView?id=sales.mth_publish_localized_content.htm&language=en_US&type=5 "After you receive the localized backpack and confirm that the appropriate updates are complete, set up a release and preview the translated content. Then, publish the release.")
-   [Add Content to a Release from Trailmaker Content](https://help.salesforce.com/s/articleView?id=sales.mth_add_content_to_release_from_tm_content.htm&language=en_US&type=5 "After you create your module and quizzes and assign all the necessary metadata, add the content to a release.")

Did this article solve your issue?

Let us know so we can improve!

YesNo