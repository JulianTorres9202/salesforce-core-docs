---
title: "Create a Multilingual Site"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_create_site.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Create a Multilingual Site

Create a Multilingual Site[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Create a Multilingual Site

Creating a multilingual site is a multistep process. It involves defining the languages you want your site to support, adding translated content for each language, and letting your site visitors choose their preferred language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To add and manage language options: | 
Site.com Publisher User field enabled on the user detail page

AND

Site administrator or designer role assigned at the site level

 |
| To edit language content: | Site.com Publisher User or Contributor User field enabled on the user detail page and any role assigned at the site level |

1.  Set the default site language. It's important that you set a default language before you add translated content to your site.
2.  Add languages to the site.
3.  Set options for each language, such as the display language and fallback language.
4.  Add content for each site language using one of these steps.
    -   Edit the page content for each language directly.
    -   Export the content for translation and then import the translated content.
5.  Add a Language Selector page element to your site pages, so authenticated site users can choose their preferred language.
6.  If you have a self-service community built on the Customer Service template, add the Language Selector component to your community pages. This component lets guest users (users who aren't logged in) choose their preferred language.

Tip After you add language-specific content to your site, you can share a separate preview URL for each language. Switch to the desired language in the Site.com Studio language selector and click **View Anonymous Preview**. Then copy the link to send it to your reviewers.

#### See Also

-   [Multilingual Sites Overview](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_overview.htm&language=en_US&type=5 "Site.com Studio lets you to create different language versions of your site. And because all languages are maintained within the site, you don't need to create and manage a separate site for each language.")
-   [About Editing Language Content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_picker.htm&language=en_US&type=5 "The default language is the language in which your site initially displays. By default, it's set to English (US), and it serves as the starting point when you add new languages. So for example, if you build your site and then add French as a site language, the French version initially contains English (US) content until you replace it with French-specific content.")

Did this article solve your issue?

Let us know so we can improve!

YesNo