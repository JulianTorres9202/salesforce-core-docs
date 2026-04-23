---
title: "Work with Translation Files"
source: "https://help.salesforce.com/s/articleView?id=platform.translation_file_description.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Work with Translation Files

Work with Translation Files[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Extend Salesforce with Clicks, Not Code](https://help.salesforce.com/s/articleView?id=platform.extend_click_intro.htm&language=en_US&type=5)

# Work with Translation Files

Translate metadata labels or data translation text, or review existing translations, with XML Localization Interchange File Format (.xlf) or Salesforce Translation Format (.stf) files.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Metadata translation available in: Salesforce Classic and Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Data translation applies to: B2B Commerce</td></tr></tbody></table>

Translation files can contain metadata translations or data translations. Metadata translations are for customizations that you made to your Salesforce organization, such as custom picklist values and custom field labels. Data translations are for the data stored within fields, such as the text in the Product object’s Name and Description fields.

For metadata and data translation files, there are three file types.

-   Source: Use to translate labels for the first time.
-   Outdated and untranslated: Use to translate labels after the first translation pass.
-   Bilingual: Use to review and edit translations.

Translation files are identified with either the .xlf or .stf extension. Salesforce recommends the XML Localization Interchange File Format (.xlf) for translation files.

-   **[Considerations for Working with Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_considerations.htm&language=en_US&type=5)**  
    Review some important considerations to ensure that your edited translation file can be successfully imported.
-   **[Source Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_source.htm&language=en_US&type=5)**  
    Use the Source file to translate an organization's labels or data for the first time. The Source file contains labels for all of a Salesforce org's translatable metadata or data in the org's default language.
-   **[Outdated and Untranslated Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_outdated.htm&language=en_US&type=5)**  
    Use the Outdated and untranslated file to translate labels or data that need translation. The file includes labels or data changed since the last translation and labels that haven't been translated. One Outdated and untranslated file is generated for each language. When multiple files are generated, they're exported to a .zip file containing a file for each translation language.
-   **[Bilingual Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_bilingual.htm&language=en_US&type=5)**  
    Use the Bilingual file to review translations, edit existing translations, and add translations for labels or data that haven't been translated. One Bilingual file is generated for each translation language.
-   **[Translation File IDs and Keys](https://help.salesforce.com/s/articleView?id=platform.workbench_translation_file_keys.htm&language=en_US&type=5)**  
    Each translatable item has a unique identifier in the translation file. In .xlf files, it’s the id within a trans-unit tag. In .stf files, it’s the key. The structure of these identifiers differs for metadata and data translation files.
-   **[Flow Identifiers in Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_flow_translation_files.htm&language=en_US&type=5)**  
    In a translation file exported from Translation Workbench, a unique key or trans-unit ID attribute identifies a flow metadata label.

#### See Also

-   [Export Metadata Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export.htm&language=en_US&type=5 "To easily translate your metadata, create files for your translators that contain your Salesforce org’s translatable metadata. Examples of translatable metadata include custom field labels, report type names, and picklist values.")
-   [Export Data Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export_data.htm&language=en_US&type=5 "If data translation is enabled in your Salesforce org, you can create files for your translators that contain your org’s data translations. Examples of translatable data include B2B Commerce Product names and data stored in custom fields.")
-   [Import Translated Files](https://help.salesforce.com/s/articleView?id=platform.workbench_import.htm&language=en_US&type=5 "Import and update the translations for your Salesforce org’s metadata, such as custom fields, report types, and picklist values. Or import and update data translations, such as Product names. Typically, you export translation files from Salesforce, then send them to outside translators or a translation agency for bulk translation activities. You then import the translated files.")

Did this article solve your issue?

Let us know so we can improve!

YesNo