---
title: "Create a Multilingual Site"
source: "https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_create.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Create a Multilingual Site

Create a Multilingual Site[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Create a Multilingual Site

Creating a multilingual site involves a few main steps. Define the languages that you want your site to support. Add translated content for each language. And enable site visitors to choose their preferred language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Experience Builder sites accessed through Lightning Experience, Salesforce Classic, and mobile devices, and is available in <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> editions.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To create an Experience Cloud site: | Create and Set Up Experiences AND View Setup and Configuration |
| To customize or publish an Experience Cloud site: | 
-   Create and Set Up Experiences AND View Setup and Configuration AND be a member of the site
    
    OR
    
-   View Setup and Configuration AND be a member of the site AND have appropriate [role-based site access](https://help.salesforce.com/s/articleView?id=experience.networks_access_control_overview.htm&language=en_US&type=5)

 |

Here’s an overview of the steps to take to create a multilingual site.

1.  [Set the default language](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_default.htm&language=en_US&type=5#community_builder_multilingual_default "The default language is the language that’s used in a site before a user has selected another language. By default, the default language is set to English (US).") for your site. It’s important to set the default language before you add translated content to your site.
2.  [Add languages](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_add.htm&language=en_US&type=5#community_builder_multilingual_add "Add the languages that you want your site to support.") to the site.
3.  [Set options](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_settings.htm&language=en_US&type=5#community_builder_multilingual_settings "After you add Experience Builder sites languages, you can define separate settings for each language.") for each language, such as the display label and fallback language.
4.  [Export and prepare the content](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_export.htm&language=en_US&type=5#community_builder_multilingual_export "Export and prepare Experience Builder site content as one or multiple .xml files. Prepare the files for translation by creating nodes for specific languages. Then send the file to your translation service."), and send it for translation. Alternatively, you can [translate content directly on the page](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_editing_about.htm&language=en_US&type=5 "Experience Builder provides its own language menu that you can use to switch between languages as you edit content on each page. Switch languages and provide spot translations, like fixing a typo. You can also use this method for full page translations instead of exporting and importing site content.") in Experience Builder.
5.  [Import the translated content](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_import.htm&language=en_US&type=5#community_builder_multilingual_import "After your translation service has completed the translations, import the translated .xml file into your Experience Builder site.").
6.  Add a [Language Selector](https://help.salesforce.com/s/articleView?id=experience.rss_language_picker.htm&language=en_US&type=5#rss_language_picker "Add the Language Selector component to multilingual sites so guest users can select their preferred language on public site pages.") component to your site pages, so unauthenticated users can choose their preferred language.
    
    Tip Consider offering users a way to get instant translations of feed items. (Feed items include posts, questions, polls, and their comments, answers, and replies.) For more information, see [Add a Translate Button to Feed Items in Experience Builder Sites](https://help.salesforce.com/s/articleView?id=experience.networks_chatter_translate.htm&language=en_US&type=5 "A translation setting in Experience Builder puts a Translate with Google menu on every feed item. Translations are offered through a Google Cloud Translation API key that you provide.").
    

#### See Also

-   [Best Practices and Considerations for Multilingual Sites](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_best_practices.htm&language=en_US&type=5 "Keep these practices and considerations in mind when you’re setting up a multilingual site.")

Did this article solve your issue?

Let us know so we can improve!

YesNo