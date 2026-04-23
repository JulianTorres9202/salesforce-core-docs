---
title: "Bulk Translation for a B2B Store"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_bulk_translate_b2b_store.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Bulk Translation for a B2B Store

Bulk Translation for a B2B Store[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Bulk Translation for a B2B Store

To accomplish bulk translations of B2B store metadata and Product, Category, and Promotion fields, use the Translation Workbench source export option. The Translation Workbench supports the XML Localization Interchange File Format (XLIFF) and the Salesforce Translation File (STF) file formats. Salesforce recommends that you use the XLIFF format.

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

Bulk translations from source files speeds up the localization process and helps maintain the quality and relevance of your content. The XLIFF translation source files contain the original metadata and Product, Category, and Promotion fields from your B2B store. The standardized format of the XLIFF file makes it easy for translators to understand the context and provide accurate translations. Translations are easily imported back into the Translation Workbench. After you import XLIFF file, the localized content is added to the system. This integration makes sure that all translated content is consistent with the original context and branding. It also provides a positive experience for users across various regions.

For small translation jobs, you can add metadata translations with the Translation Workbench metadata feature. You can manually add Product, Category, and Promotion field translations through the Commerce App. See [Manually Localize B2B Store Labels](https://help.salesforce.com/s/articleView?id=commerce.comm_translate_store_labels_manually.htm&language=en_US&type=5).

-   **[XLIFF File Format for Importing Commerce Translations](https://help.salesforce.com/s/articleView?id=commerce.comm_xliff_file_format_import_translations.htm&language=en_US&type=5)**  
    The Translation Workbench supports the XML Localization Interchange File Format (XLIFF) and Salesforce Translation File (STF) file formats.
-   **[Structure of the Store Metadata Translation Source File](https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_metadata_translation_source_file.htm&language=en_US&type=5)**  
    In situations where Salesforce doesn’t provide default metadata translations, you can localize your store’s metadata and the custom functionality that you build.
-   **[Structure of the Store Data Translation Source File](https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_data_translation_source_file.htm&language=en_US&type=5)**  
    The XLIFF source files for products, categories, and promotions include each object’s translatable fields. Each data source file’s element structure is specific to your store’s products, categories, or promotions. To avoid missed translations, download the XLIFF source files after your products, categories, and promotions are set for your store launch.

#### See Also

-   [Enable Translation Workbench](https://help.salesforce.com/s/articleView?id=commerce.comm_translation_workbench.htm&language=en_US&type=5 "To assist with localizing B2B store information, enable the Translation Workbench and add the languages that you want to use in your stores.")
-   [XLIFF File Format for Importing Commerce Translations](https://help.salesforce.com/s/articleView?id=commerce.comm_xliff_file_format_import_translations.htm&language=en_US&type=5 "The Translation Workbench supports the XML Localization Interchange File Format (XLIFF) and Salesforce Translation File (STF) file formats.")
-   [Structure of the Store Metadata Translation Source File](https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_metadata_translation_source_file.htm&language=en_US&type=5 "In situations where Salesforce doesn’t provide default metadata translations, you can localize your store’s metadata and the custom functionality that you build.")
-   [Structure of the Store Data Translation Source File](https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_data_translation_source_file.htm&language=en_US&type=5 "The XLIFF source files for products, categories, and promotions include each object’s translatable fields. Each data source file’s element structure is specific to your store’s products, categories, or promotions. To avoid missed translations, download the XLIFF source files after your products, categories, and promotions are set for your store launch.")

Did this article solve your issue?

Let us know so we can improve!

YesNo