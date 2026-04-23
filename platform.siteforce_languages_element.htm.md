---
title: "Adding a Language Selector Page Element"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_element.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Adding a Language Selector Page Element

Adding a Language Selector Page Element[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Adding a Language Selector Page Element

The language selector lets your site visitors choose their preferred language when viewing a site.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To add and manage language options: | 
Site.com Publisher User field enabled on the user detail page

AND

Site administrator or designer role assigned at the site level

 |

After you add languages to your site, you need to let site visitors select their preferred language from the list of languages you defined in the Languages view.

Tip To save time, add the language selector to your site's page templates.

When the page is open:

1.  Drag a **Language Selector** from the Page Elements pane onto the page.
    
    Site visitors will see a Change Site Language drop-down list when they visit the page.
    
2.  Set properties for the language selector:
    
    | Property | Description |
    | --- | --- |
    | Do Not Translate | Select this checkbox if you want the text in the Label field to remain the same for all languages. |
    | Label | 
    The label that appears beside the Language Selector page element when it's added to a page. “Change Site Language” is the default text.
    
    The text is translatable, so you can either choose a language in the Site.com Studio language selector and update the text for each language, or export all site content for translation.
    
     |
    | Home Page URL | Redirects site visitors to a different page when they choose a language. The URL is the same for all languages. |
    

#### See Also

-   [Language-Aware Properties](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_prop.htm&language=en_US&type=5 "Several properties in the Properties pane are language aware, meaning they can store different values for each language.")

Did this article solve your issue?

Let us know so we can improve!

YesNo