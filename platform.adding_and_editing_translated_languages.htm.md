---
title: "Add Translated Languages and Translators"
source: "https://help.salesforce.com/s/articleView?id=platform.adding_and_editing_translated_languages.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Add Translated Languages and Translators

Add Translated Languages and Translators[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Add Translated Languages and Translators

Add languages for translation, assign translators for each language, and activate or deactivate a language’s translations.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To add or edit languages: | Manage Translation |
| To assign translators: | Manage Translation |

Note The Manage Translation permission is enabled by default in the System Administrator profile.

Before adding a language for translation, you must select languages for your org and enable Translation Workbench.

[](https://help.salesforce.com/s?language=en_US)

1.  From Setup, in the Quick Find box, enter Translation Language Settings, and then select **Translation Language Settings**.
2.  To activate a new language, click **Add**. Or to change an existing supported language, click **Edit**.
3.  If adding a language, choose a language.
4.  To make the entered translations available to your users, select Active. Users can change their personal language anytime, regardless of whether it's active in the Translation Workbench. Selecting Active makes the translations available to the users in that language.
    
    We recommend that you don't make a language active until the translators have translated all values.
    
    Note If you installed a managed package that includes translations, those translated values appear to users regardless of whether the language is active on the Translation Language Settings Setup page.To override metadata translations delivered by a managed package for custom objects, see Override Translations in Second-Generation Managed Packages and Unlocked Packages.
    
5.  To assign translators for this language, select them from the Available List, and click **Add**. If you don't see the member that you want to add, enter keywords in the search box, and click **Find**.
    
    Important Ensure that all translators have the View Setup and Configuration permission so that they can begin translating. Users can only translate languages that they're assigned to.
    
6.  Save your changes.

#### See Also

-   [Select Languages for Your Org](https://help.salesforce.com/s/articleView?id=xcloud.admin_select_languages_for_your_org.htm&language=en_US&type=5)
-   [Enable or Disable Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.customize_wbench.htm&language=en_US&type=5 "Translation Workbench allows you to specify languages for translation, assign translators, and manage your translations through the workbench or bulk translation.")
-   [Override Translations in Second-Generation Managed Packages and Unlocked Packages](https://help.salesforce.com/s/articleView?id=platform.entering_translated_terms_in_packages.htm&language=en_US&type=5 "You can override metadata translations for custom objects in namespaced unlocked packages and second-generation managed packages. For example, override the label on a custom field or workflow task.")

Did this article solve your issue?

Let us know so we can improve!

YesNo