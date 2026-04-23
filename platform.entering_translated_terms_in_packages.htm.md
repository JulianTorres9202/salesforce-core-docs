---
title: "Override Translations in Second-Generation Managed Packages and Unlocked Packages"
source: "https://help.salesforce.com/s/articleView?id=platform.entering_translated_terms_in_packages.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Override Translations in Second-Generation Managed Packages and Unlocked Packages

Override Translations in Second-Generation Managed Packages and Unlocked Packages[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Override Translations in Second-Generation Managed Packages and Unlocked Packages

[](https://help.salesforce.com/s?language=en_US)You can override metadata translations for custom objects in namespaced unlocked packages and second-generation managed packages. For example, override the label on a custom field or workflow task.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To override metadata translations: | 
View Setup and Configuration

AND

Customize Application

 |

Note Overriding translations in second-generation managed packages and unlocked packages has limitations:

-   You can’t override translations for standard objects in packages.
-   You can’t override translations for global picklist value sets.
-   You can’t override data translations.

If you installed a managed package that includes translations, those translated values appear to users regardless of whether the language is active on the Translation Language Settings Setup page. Before you can override those translations, you must select languages for your org and enable Translation Workbench.

1.  From Setup, in the Quick Find box, enter Override, and then select **Override**.
2.  Select the Package that you’re overriding.
3.  Select the Language that you're entering your overrides in.
    
    Note The Language list shows the languages that meet these criteria:
    
    -   The language is in the package that’s associated with this namespace.
    -   There is at least one translation for the language, or it’s the package default language.
    
4.  Select a Setup Component. See Metadata Available for Translation for a list of translatable components.
5.  Depending on the setup component, select the next options.
    
    The aspect is a part of the setup component that you can translate. For example:For global value sets and picklist values, you can translate inactive values by selecting **Show Inactive Values**.
    
    -   Workflow tasks have an object (for example, Account or Contact) and aspect (Subject or Comment).
    -   Custom Report Types have a custom report type entity (Custom Report Type, Custom Report Type Column, or Custom Report Type Layout Section) and aspect (field label or description).
    -   Flows have a flow type (Flow and Autolaunched Flow), a flow name, and a flow component (Definition, Version, Screen Info, Screen Field, and Choice). Flow components can have a flow version, screen, or aspect.
6.  To enter new values, double-click in the translation column. You can press TAB to advance to the next editable field or SHIFT-TAB to go to the previous editable field.
    
    Note The Out of Date column indicates the possibility that the term needs translation because the primary label has been updated. When editing a button or link label, you see the Button or Link Name column, which is used to refer to the component when using SOAP API.
    
7.  Click **Save**.

#### See Also

-   [Select Languages for Your Org](https://help.salesforce.com/s/articleView?id=xcloud.admin_select_languages_for_your_org.htm&language=en_US&type=5)
-   [Enable or Disable Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.customize_wbench.htm&language=en_US&type=5 "Translation Workbench allows you to specify languages for translation, assign translators, and manage your translations through the workbench or bulk translation.")
-   [Metadata Available for Translation](https://help.salesforce.com/s/articleView?id=platform.translatable_customizations.htm&language=en_US&type=5 "You can translate metadata labels only for certain Salesforce Setup components.")

Did this article solve your issue?

Let us know so we can improve!

YesNo