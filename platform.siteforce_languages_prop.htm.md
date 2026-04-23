---
title: "Language-Aware Properties"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_prop.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Language-Aware Properties

Language-Aware Properties[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Language-Aware Properties

Several properties in the Properties pane are language aware, meaning they can store different values for each language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

If you don't specify language-specific properties for a page or page element, the property values of the default languages are used instead.

| Property | Applies To | Description |
| --- | --- | --- |
| Alternative Text | Image | Used by screen reader users or as a substitute if the browser can't display the image. It can also help with search engine optimization (SEO). |
| [](https://help.salesforce.com/s?language=en_US)Do Not Translate | 
-   Content Block
-   Custom Code
-   Data Element
-   Form
-   Input Fields
-   Image
-   Language Selector
-   Page

 | 

[](https://help.salesforce.com/s?language=en_US)Prevents the item's content from being translated. When selected, the globe icon () is removed from language-aware properties, indicating that they no longer support language-specific content.

[](https://help.salesforce.com/s?language=en_US)If you add language-specific content and subsequently enable this property, your language-specific content is simply hidden. If you disable the property again, the content reappears.

 |
| [](https://help.salesforce.com/s?language=en_US)Home Page URL | Language Selector | [](https://help.salesforce.com/s?language=en_US)Redirects site visitors to a different page when they choose a language. The URL is the same for all languages. |
| Image Asset | Image | 

Lets you specify the image to display for the selected language.

For example, with English (US) selected in the Site.com Studio language selector, select the English version of an imported image. Then, to enter a French version of the same image, select French in the language selector and select the French image.

 |
| [](https://help.salesforce.com/s?language=en_US)Label | Language Selector | 

[](https://help.salesforce.com/s?language=en_US)The label that appears beside the Language Selector page element when it's added to a page. “Change Site Language” is the default text.

[](https://help.salesforce.com/s?language=en_US)The text is translatable, so you can either choose a language in the Site.com Studio language selector and update the text for each language, or export all site content for translation.

 |
| Navigation Name | Page | The page name that appears in a navigation menu. |
| Title | Page | The title that appears in the title bar of browser windows. |
| Visible in Live Site | Page | 

If you add a menu to your site, controls whether the page appears in the menu for the selected language. Additionally, the page is no longer accessible via its language-specific URL.

If Do Not Translate is also enabled, the status of Visible in Live Site applies to all languages.

 |

#### See Also

-   [Edit Language Content on the Page](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_editing.htm&language=en_US&type=5 "The Site.com Studio language selector lets you switch between languages as you edit content on each page. Contributors, designers, and site administrators can each add language-specific content to a page using the language selector.")
-   [About Editing Language Content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_picker.htm&language=en_US&type=5 "The default language is the language in which your site initially displays. By default, it's set to English (US), and it serves as the starting point when you add new languages. So for example, if you build your site and then add French as a site language, the French version initially contains English (US) content until you replace it with French-specific content.")

Did this article solve your issue?

Let us know so we can improve!

YesNo