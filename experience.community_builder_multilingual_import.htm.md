---
title: "Import Translated Content"
source: "https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_import.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Import Translated Content

Import Translated Content[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Import Translated Content

After your translation service has completed the translations, import the translated .xml file into your Experience Builder site.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Experience Builder sites accessed through Lightning Experience, Salesforce Classic, and mobile devices, and is available in <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> editions.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To customize or publish an Experience Cloud site: | 
-   Create and Set Up Experiences AND View Setup and Configuration AND be a member of the site
    
    OR
    
-   View Setup and Configuration AND be a member of the site AND have appropriate [role-based site access](https://help.salesforce.com/s/articleView?id=experience.networks_access_control_overview.htm&language=en_US&type=5)

 |

Don't update your site’s default content until after you import the translated content. The translated file contains the original default content and the translated content. When you import the translated file, the import overwrites any changes that you made to the default content while the content was with your translation service.

Note If you exported your site content for translation before Winter ’22, you can’t import the resulting translated file. To ensure a successful import, export your site content again and translate it in this more recent .xml file.

1.  In Experience Builder, click  | **Languages**.
2.  Click **Import Translation**.
3.  Browse to the file or drag it onto the window.
    
    For files under 1 MB, a message tells you whether the content was imported successfully. For files over 1 MB, you receive an email when the import process finishes.
    

Warning Import overwrites the current translation values in your site. Before you import an .xml file, ensure that the file matches the expected format and is well formed.

After you import the translated content, test your pages to make sure that content displays correctly. Use the language selector to view each page in a supported language.

#### See Also

-   [Export Language Content](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_export.htm&language=en_US&type=5 "Export and prepare Experience Builder site content as one or multiple .xml files. Prepare the files for translation by creating nodes for specific languages. Then send the file to your translation service.")

Did this article solve your issue?

Let us know so we can improve!

YesNo