---
title: "Exporting Language Content"
source: "https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_export.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Exporting Language Content

Exporting Language Content[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Exporting Language Content

Export one or more site languages as an .xml file that you can send to your translation service.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Salesforce Classic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p lwc-3eigj2skqo3="">Available for purchase in: <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Unlimited</strong> Editions</p><p style="margin-bottom:0;" lwc-3eigj2skqo3="">Available (with limitations) in: <strong lwc-3eigj2skqo3="">Developer</strong> Edition</p></td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To add and manage language options: | 
Site.com Publisher User field enabled on the user detail page

AND

Site administrator or designer role assigned at the site level

 |

1.  In the Languages view on the Overview tab, click  | **Export Content for Translation**.
2.  Select the language content that you want to export for translation. (Use CTRL+click to select multiple items.)
3.  Optionally, enter a different filename. The default name is languages.xml.
4.  Click **OK**.
5.  If required by your browser, choose where to save the file.

After you export the .xml file, you can send it for translation.

Example The .xml file contains a time stamp attribute that records the time of the export, and encloses all translatable content in CDATA sections, as shown in this example.

When you receive the translated .xml file, import it back into the site.

#### See Also

-   [Importing Translated Content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_import.htm&language=en_US&type=5 "You can import a translated .xml file back into your site after your translation service has completed the translations.")
-   [About Editing Language Content](https://help.salesforce.com/s/articleView?id=platform.siteforce_languages_picker.htm&language=en_US&type=5 "The default language is the language in which your site initially displays. By default, it's set to English (US), and it serves as the starting point when you add new languages. So for example, if you build your site and then add French as a site language, the French version initially contains English (US) content until you replace it with French-specific content.")

Did this article solve your issue?

Let us know so we can improve!

YesNo