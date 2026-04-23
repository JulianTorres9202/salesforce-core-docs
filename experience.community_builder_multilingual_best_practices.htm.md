---
title: "Best Practices and Considerations for Multilingual Sites"
source: "https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_best_practices.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Best Practices and Considerations for Multilingual Sites

Best Practices and Considerations for Multilingual Sites[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Best Practices and Considerations for Multilingual Sites

Keep these practices and considerations in mind when you’re setting up a multilingual site.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Experience Builder sites accessed through Lightning Experience, Salesforce Classic, and mobile devices, and is available in <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> editions.</td></tr></tbody></table>

## General Best Practices and Considerations

-   Set the site’s default language before you begin adding translated content to your site.
-   For each translation, export a separate Languages.xml file to reduce the chance of overwriting any existing translations when importing new translations. For easier identification, we recommend renaming each file to include its country code—for example, languages\_de.xml, languages\_fr\_ca.xml.
-   When preparing files for translation, ensure that the file contains the default language and only one other language. When you import the file after translation, this best practice helps avoid overwriting any other languages.
-   If possible, avoid updating the site’s default content until after you receive and import your translated content. Because the translated file contains the original default content and the translated content, when you import the file, you overwrite any updates made in the interim.
-   If you decide to change a site’s default language after you add translated content, do so in this order:
    
    -   Export site content.
    -   Change the default language.
    -   Import the exported file.
    
    You export first because changing the default language can overwrite existing translations. Export first to preserve your original default language and your translations. Then, after changing the default, import translations to restore them.
    
    Here’s how it works. Let’s say that you make English the default language and add French as a site language. After you add the translated French content, you decide to change the default site language to French. To preserve your original default language and existing translations, you must first export site content. Then select French as the default site language, and import content back into the site.
    
-   For custom components, when you make a new property available for edit in Experience Builder, keep this consideration in mind for translations: If the component is in use on a page in Experience Builder, delete the component from the page and replace it with the updated version. Otherwise, when you export the site content for translation, the property that you added is omitted for that component instance in the exported file. If the component contains content that’s already translated, export the site content first to preserve the existing translation. Then replace the component with the updated version. For more information, see [Aura Component Bundle Design Resources](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/components_config_for_app_builder_design_files.htm) or, for Lightning web components, [Configure a Component for Experience Builder](https://developer.salesforce.com/docs/component-library/documentation/en/lwc/use_config_for_community_builder).

## Best Practices and Considerations for Authenticated Users

-   For pages that require authentication, page content appears in the authenticated user’s profile language.
-   When authenticated users want to view a multilingual site in another language, their best option is to view the site as a guest user. Or, these users can change their profile language. Don’t edit the query parameters in a site’s URL to update the site’s language.

## Best Practices and Considerations for Guest Users

-   Add a language selector to all public pages, and make it easy to spot. It's the only way that guest users and unauthenticated visitors can select another language.
-   Customized labels and Knowledge articles use the translations that the site admin added in Translation Workbench.

#### See Also

-   [_Blog post_: Localization within Experience Cloud Sites](https://www.learnexperiencecloud.com/article/Localization-within-Experience-Cloud-Sites)
-   [Language Selector](https://help.salesforce.com/s/articleView?id=experience.rss_language_picker.htm&language=en_US&type=5 "Add the Language Selector component to multilingual sites so guest users can select their preferred language on public site pages.")

Did this article solve your issue?

Let us know so we can improve!

YesNo