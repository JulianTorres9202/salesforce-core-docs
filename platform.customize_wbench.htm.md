---
title: "Enable or Disable Translation Workbench"
source: "https://help.salesforce.com/s/articleView?id=platform.customize_wbench.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Enable or Disable Translation Workbench

Enable or Disable Translation Workbench[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Enable or Disable Translation Workbench

Translation Workbench allows you to specify languages for translation, assign translators, and manage your translations through the workbench or bulk translation.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To enable and disable Translation Workbench: | Customize Application |

1.  From Setup, in the Quick Find box, enter Translation Language Settings, and then select **Translation Language Settings**.
2.  On the welcome page, click **Enable**.

Enabling Translation Workbench makes these changes to your Salesforce org. If a customized component doesn’t have a translated value, the component uses the org’s default language. When you deactivate a language, all translations for that language are still available in Translation Workbench. However, users with that language selected see the org’s default language values.

-   The Manage Translation systems permission is available in permission sets.
-   You must edit picklist values individually. You can’t mass-edit existing picklist values, but you can still mass-add new values.
-   When picklist values are sorted alphabetically, the values are alphabetical by the user's locale.
-   Reports have a Filter Language dropdown list in the Filters pane of the report builder. Selecting a language filters on translated strings for any filter criteria that use the starts with, contains, or doesn’t contain operator.
-   Import files have a Language dropdown list, and all records and values within the import file must be in the selected language.
-   Web-to-Lead and Web-to-Case have a Language dropdown list before you generate the HTML.

[](https://help.salesforce.com/s?language=en_US)To disable Translation Workbench, from Setup, in the Quick Find box, enter Translation Language Settings, and then select **Translation Language Settings**. Click **Disable**.

Note In a Developer org with a managed package containing translations, Translation Workbench can’t be disabled after it’s enabled.

#### See Also

-   [Supported Languages](https://help.salesforce.com/s/articleView?id=xcloud.faq_getstart_what_languages_does.htm&language=en_US&type=5)
-   [Language, Locale, and Currency Settings](https://help.salesforce.com/s/articleView?id=xcloud.admin_language_locale_currency.htm&language=en_US&type=5)
-   [Rename Object, Tab, and Field Labels](https://help.salesforce.com/s/articleView?id=platform.customize_rename.htm&language=en_US&type=5 "You can change the name of almost any object, field, or tab in Salesforce. This simple adjustment lets you continue using the terminology your users already know and helps them transition to using Salesforce. However, Salesforce Help and most pages in Setup always display the original names for standard objects, fields, and tabs.")

Did this article solve your issue?

Let us know so we can improve!

YesNo