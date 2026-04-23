---
title: "Translate Metadata Labels"
source: "https://help.salesforce.com/s/articleView?id=platform.entering_translated_terms.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Metadata Labels

Translate Metadata Labels[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Translate Metadata Labels

Create and update metadata translations for customizations you make to your Salesforce organization, such as custom picklist values and custom field labels.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To translate terms: | 
View Setup and Configuration

AND

Be designated as a translator

 |

Note Entering translations through Translation Workbench has limitations, so note the following.

-   Use the rename tabs and labels interface for standard object translation. Standard objects and custom object names aren’t available in Translation Workbench.
-   Manage data translations through the Translation tab within Product or through the Export and Import options in Translation Workbench. Only metadata translations are available for translation via the Translate Setup page.

Before translating metadata labels, you must select languages for your org, enable Translation Workbench, and add translated languages and translators.

1.  From Setup, in the Quick Find box, enter Translate, and then select **Translate**.
2.  Select the Language you're translating into.
3.  Select a Setup Component. See Metadata Available for Translation for a list of translatable components.
4.  Depending on the setup component, select the next options.
    
    The aspect is a part of the setup component that you can translate. For example:For global value sets and picklist values, you can translate inactive values by selecting **Show Inactive Values**.
    
    -   Workflow tasks have an object (for example, Account or Contact) and aspect (Subject or Comment).
    -   Custom Report Types have a custom report type entity (Custom Report Type, Custom Report Type Column, or Custom Report Type Layout Section) and aspect (field label or description).
    -   Flows have a flow type (Flow and Autolaunched Flow), a flow name, and a flow component (Definition, Version, Screen Info, Screen Field, and Choice). Flow components can have a flow version, screen, or aspect.
    
5.  To enter new values, double-click in the translation column. You can press Tab to advance to the next editable field or Shift+Tab to go to the previous editable field.
    
    Note The Out of Date column indicates the possibility that the label needs translating because the primary label has been updated. When editing a button or link label, you see the Button or Link Name column, which is used to refer to the component when using SOAP API.
    
6.  [](https://help.salesforce.com/s?language=en_US)Click **Save**.

If a customized component doesn’t have a translated value, the component uses the org’s default language. When you deactivate a language, all translations for that language are still available in Translation Workbench. However, users with that language selected see the org’s default language values.

#### See Also

-   [Select Languages for Your Org](https://help.salesforce.com/s/articleView?id=xcloud.admin_select_languages_for_your_org.htm&language=en_US&type=5)
-   [Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.workbench.htm&language=en_US&type=5 "Use Translation Workbench to maintain translated values for metadata and data labels in your Salesforce org. Specify languages for translation and assign translators for each language. Manage translated values for any Salesforce supported language. Translators can maintain translations directly through the workbench, or you can export translation files for bulk translation imports.")
-   [Rename Object, Tab, and Field Labels](https://help.salesforce.com/s/articleView?id=platform.customize_rename.htm&language=en_US&type=5 "You can change the name of almost any object, field, or tab in Salesforce. This simple adjustment lets you continue using the terminology your users already know and helps them transition to using Salesforce. However, Salesforce Help and most pages in Setup always display the original names for standard objects, fields, and tabs.")
-   [Metadata Available for Translation](https://help.salesforce.com/s/articleView?id=platform.translatable_customizations.htm&language=en_US&type=5 "You can translate metadata labels only for certain Salesforce Setup components.")

Did this article solve your issue?

Let us know so we can improve!

YesNo