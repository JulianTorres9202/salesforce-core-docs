---
title: "Setting the Default Language"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_default.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Setting the Default Language

Setting the Default Language[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Setting the Default Language

The default language is the language in which your site initially displays. By default, it's set to English (US), and it serves as the starting point when you add new languages.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To add and manage language options: | 
Site.com Publisher User field enabled on the user detail page

AND

Site administrator or designer role assigned at the site level

 |

It's important to set the default language before you add any language content to your site. This setting is not associated with the default language setting in your Salesforce organization.

1.  Click **Site Configuration** | **Languages** on the Overview tab.
2.  Select a language in the Default Site Language drop-down list.

Note If you decide to change the default language after you add translated content, you must first export the translated content, then change the default language, and finally, import the content back into your site. Otherwise the translated content won't appear for the newly selected default language.

For example, let's say you make English the default site language and add French as a site language. After you add content in both English and French, you decide to change the default site language to French. To preserve the French content, you must first export it. Then, select French as the default site language before importing the French content back into the site.

#### See Also

-   [Adding Languages](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_add.htm&language=en_US&type=5 "Add the languages you want your site to support.")
-   [Setting Language Options](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_settings.htm&language=en_US&type=5 "After you add site languages in the Languages view, you can define separate settings for each one.")

Did this article solve your issue?

Let us know so we can improve!

YesNo