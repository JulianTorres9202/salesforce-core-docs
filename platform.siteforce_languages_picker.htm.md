---
title: "About Editing Language Content"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_picker.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# About Editing Language Content

About Editing Language Content[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# About Editing Language Content

[](https://help.salesforce.com/s?language=en_US)The default language is the language in which your site initially displays. By default, it's set to English (US), and it serves as the starting point when you add new languages. So for example, if you build your site and then add French as a site language, the French version initially contains English (US) content until you replace it with French-specific content.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

After you add a language to your site, the Site.com Studio language selector appears on the toolbar. It lets you switch between languages as you edit content on each page. For example, if you add French and Spanish to your site, the language selector displays French, Spanish, and English (US).

Content blocks display icons to let you know whether content for the selected language has been replaced.

[](https://help.salesforce.com/s?language=en_US)

-   A warning icon () indicates that the text that has not yet been replaced.
-   A globe icon () indicates that the content has been replaced.

In addition, several page elements have [language aware properties](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_prop.htm&language=en_US&type=5 "Several properties in the Properties pane are language aware, meaning they can store different values for each language."), meaning they can store different values for each language. These properties are indicated in the Properties pane by a globe icon ().

You can add content for each site language one of two ways:

-   [Edit the page content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_editing.htm&language=en_US&type=5 "The Site.com Studio language selector lets you switch between languages as you edit content on each page. Contributors, designers, and site administrators can each add language-specific content to a page using the language selector.") for each language directly using the Site.com Studio language selector.
-   [Export the content for translation](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_export.htm&language=en_US&type=5 "Export one or more site languages as an .xml file that you can send to your translation service.") and then [import the translated content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_import.htm&language=en_US&type=5 "You can import a translated .xml file back into your site after your translation service has completed the translations.") back into the site.

## Language Display Order

After you add language-specific content to your site, content on the page is displayed in the following order, depending on which language content is available:

1.  Selected language
2.  Fallback language
3.  Default language

For example, if you delete the French contents of a content block, and Spanish is the fallback language, the Spanish content is displayed rather than the default language content. In turn, if you delete the Spanish content, then the default language content is displayed.

## Language–Aware Page Elements

The following page elements support translated content:

-   Content Block
-   Custom Code
-   Data Element
-   Form
-   Input Fields
-   Image
-   Language Selector

#### See Also

-   [Language-Aware Properties](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_prop.htm&language=en_US&type=5 "Several properties in the Properties pane are language aware, meaning they can store different values for each language.")

Did this article solve your issue?

Let us know so we can improve!

YesNo