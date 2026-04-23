---
title: "Set the Default Language for Your Aura Site"
source: "https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_default.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Set the Default Language for Your Aura Site

Set the Default Language for Your Aura Site[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Set the Default Language for Your Aura Site

The default language is the language that’s used in a site before a user has selected another language. By default, the default language is set to English (US).

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Applies to: <a target="_blank" href="https://help.salesforce.com/s/articleView?id=experience.exp_cloud_basics_glossary.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">Aura sites</a></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To customize or publish an Experience Cloud site: | 
-   Create and Set Up Experiences AND View Setup and Configuration AND be a member of the site
    
    OR
    
-   View Setup and Configuration AND be a member of the site AND have appropriate [role-based site access](https://help.salesforce.com/s/articleView?id=experience.networks_access_control_overview.htm&language=en_US&type=5)

 |

Before you add any language content to your site, you must set the site’s default language. A site’s default language isn’t the same as the default language setting in your Salesforce org. This behavior is deliberate. Let’s say you have multiple sites and want a different default language for each. At the same time, you want your org default language to be consistent. With a separate default language for your org, it’s easy to set things up this way.

1.  In Experience Builder, click  | **Languages**.
2.  Select a language from the Default Site Language list.
    
    Note If you plan to add Salesforce CMS content to your site, it’s important that the site and the CMS workspace have the same default language so that the content appears properly. If the default languages are different, translate the content in your CMS workspace into your default site language, then add the translated content to your site.
    
3.  Optionally, click **Edit display label**, and change the way the selected language label appears. For example, you can use this opportunity to translate the language’s display label.

Important If you decide to change a site’s default language after you add translated content, do so in this order:

1.  Export site content.
2.  Change the default language.
3.  Import the exported file.

Changing the default language can overwrite existing translations. So you export first to preserve your original default language and your translations. After you change the default, you can import translations to restore them.

Here’s how it works. Let’s say you make English the default language and add French as a site language. After you add the translated French content, you decide to change the default site language to French. To preserve your original default language and existing translations, you must first export. Then, select French as the default site language, and import content back into the site.

#### See Also

-   [Add Languages to Your Aura Sites](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_add.htm&language=en_US&type=5 "Add the languages that you want your site to support.")
-   [Set Language Options](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_settings.htm&language=en_US&type=5 "After you add Experience Builder sites languages, you can define separate settings for each language.")
-   [Translate Salesforce CMS Content](https://help.salesforce.com/s/articleView?id=xcloud.cms_translations_overview.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo