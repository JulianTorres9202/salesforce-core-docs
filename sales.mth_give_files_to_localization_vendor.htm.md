---
title: "Give Content Files to a Localization Team or Vendor"
source: "https://help.salesforce.com/s/articleView?id=sales.mth_give_files_to_localization_vendor.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Give Content Files to a Localization Team or Vendor

Give Content Files to a Localization Team or Vendor[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Enablement Sites (myTrailhead)](https://help.salesforce.com/s/articleView?id=sales.mth_intro.htm&language=en_US&type=5)

# Give Content Files to a Localization Team or Vendor

To add localized content, send the backpack to your localization team or vendor. The backpack is a ZIP file, downloaded from Trailmaker, that contains the module or trail’s source files. You can send the backpack ZIP file or give the vendor access to your version control system (VCS) to download the backpack. After the vendor translates your content, the vendor can upload the backpack—updated with the localized files—to your VCS. Then, you can publish the localized content.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</td></tr></tbody></table>

| User Roles |
| --- |
| This topic supports these enablement site roles: | 
-   Release Managers
-   Localization Team or Vendor

 |

In general, complete these steps when you give your files to a localization vendor:

1.  Find the backpack for the content that you want to localize. You can:
    
    -   Access the backpack in your company’s VCS.
    -   Download the latest released version of the backpack from Trailmaker Release. To learn more, see [Download a Backpack from Trailmaker Release](https://help.salesforce.com/s/articleView?id=sales.mth_tm_release_download.htm&language=en_US&type=5 "From Trailmaker Release, you can download the backpack ZIP file for a module or trail published in your company’s enablement site. With this backpack, your content creators can easily access the latest released version of content the next time they want to update it.").
    
2.  Give the backpack with the source files to your localization vendor. To help your localization vendor complete the request more efficiently, specify which elements in the backpack you want them to translate.
3.  The localization team or vendor translates the source files and returns the backpack to you.
    
    Important
    
    -   Many localization teams and vendors use computer-aided translation tools that protect HTML, JSON, and YAML code from being edited. The translator can change content values, but can’t modify any tags, attributes, or other underlying code.
    -   If your localization team or vendor doesn’t work with such software, they can use a text editor that shows the code. However, they must take care to avoid editing code.
    -   Avoid word processors for translation because word processors can insert code artifacts that can make future edits and translations more difficult.
    -   You can’t use Trailmaker to translate content.
    
4.  When you receive the backpack with the localized content, confirm that its structure is correct by reviewing the [guidelines for localizing files in a backpack](https://help.salesforce.com/s/articleView?id=sales.mth_localize_files.htm&language=en_US&type=5 "Your localization team or vendor can localize only certain trail, module, unit, and quiz information in your backpack’s files.").

When you’re ready, add the localized backpack to an unpublished release and publish by completing the steps in [Preview and Publish Localized Content](https://help.salesforce.com/s/articleView?id=sales.mth_publish_localized_content.htm&language=en_US&type=5 "After you receive the localized backpack and confirm that the appropriate updates are complete, set up a release and preview the translated content. Then, publish the release.").

#### See Also

-   [Considerations for Languages on Your Enablement Site](https://help.salesforce.com/s/articleView?id=sales.mth_language.htm&language=en_US&type=5 "The default language for any enablement site is English, but other languages are supported. A user can select a different language, but the extent to which content is available for any language depends on whether you’ve localized and published content for that language.")
-   [Guidelines for Localizing Files in a Backpack](https://help.salesforce.com/s/articleView?id=sales.mth_localize_files.htm&language=en_US&type=5 "Your localization team or vendor can localize only certain trail, module, unit, and quiz information in your backpack’s files.")
-   [Preview and Publish Localized Content](https://help.salesforce.com/s/articleView?id=sales.mth_publish_localized_content.htm&language=en_US&type=5 "After you receive the localized backpack and confirm that the appropriate updates are complete, set up a release and preview the translated content. Then, publish the release.")
-   [Backpacks for Trails and Modules](https://help.salesforce.com/s/articleView?id=sales.mth_backpacks_on_mytrailhead.htm&language=en_US&type=5 "A backpack is a ZIP file that contains your content’s source files that you can download, back up, or upload. An individual backpack can be up to 50 MB. You can download a backpack for content that’s in your local Trailmaker Content workspace, or download a backpack for content published from Trailmaker Release.")

Did this article solve your issue?

Let us know so we can improve!

YesNo