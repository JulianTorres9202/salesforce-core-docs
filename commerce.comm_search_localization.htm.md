---
title: "Languages Supported for Search Results"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_search_localization.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Languages Supported for Search Results

Languages Supported for Search Results[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Languages Supported for Search Results

Search for B2B stores supports all languages provided by Salesforce. For D2C stores, search results are returned in the language of the store. For B2B stores, search results are returned in the language assigned to the buyer’s user account. If a buyer is configured to use a language that isn’t enabled for the store, search results, including facet and filter values, are returned in the store's default language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

Search for B2B stores supports the same languages as the [Salesforce platform](https://help.salesforce.com/s/articleView?id=xcloud.faq_getstart_what_languages_does.htm&language=en_US&type=5). However, search behavior varies based on the default language set for your [B2B](https://help.salesforce.com/s/articleView?id=commerce.comm_lang_curr_international_b2b_store.htm&language=en_US&type=5) or [D2C](https://help.salesforce.com/s/articleView?id=commerce.comm_lang_curr_international_b2c_store.htm&language=en_US&type=5) store, the translations you define for products and categories, and the language that the customer selects for browsing. To get the best search results, make sure [Translation Workbench](https://help.salesforce.com/s/articleView?id=commerce.comm_translation_workbench.htm&language=en_US&type=5) and [Data Translation](https://help.salesforce.com/s/articleView?id=commerce.comm_enable_data_translation.htm&language=en_US&type=5) are enabled, and that [translations are defined](https://help.salesforce.com/s/articleView?id=commerce.comm_create_data_translation.htm&language=en_US&type=5) for all products and languages. If you don’t define translations for all products in all languages enabled for the store, including the default language, the search returns products only when the customer searches for terms that match values in the product record detail. Search results also vary based on whether or not semantic search is enabled.

For example, consider a B2B store where the default language is Spanish. The product name on the product record page is the Spanish word for shirt, "camisa”.

A customer browsing the store selects Spanish as the language for the store. If they enter "camisa" in the search box, the product appears in the search results even if no specific Spanish translation is defined for "camisa."

Similarly, if a customer selects Korean as the language for the store but no specific Korean translation is defined for the product, entering the Spanish word "camisa" in the search returns the product in the search results.

However, if the customer selects French as the language for the store and the French translation is defined for the product, entering the Spanish word "camisa" in the search doesn’t return any results. The customer must enter the words specified in the French translation to yield results.

| Store's Default Language | Product Record Details | Customer Browsing Language | Product Translations | Search Phrase | Search Results | Search Results (Semantic Search Enabled) |
| --- | --- | --- | --- | --- | --- | --- |
|   |   | Spanish | Not defined in Spanish | camisa | Product is returned in search results. | Product is returned in search results. |
| Spanish | Product Name in Spanish: camisa | French | Product Name defined in French: chemise | camisa | Product isn't returned in search results. | Product is likely returned in search results. |
|   |   | camisa | Product is included in search results. | Product isn't included in search results. |
| Korean | Not defined in Korean | syeocheu | Product isn't included in search results. | Product is likely returned in search results. |
|   |   |   |   | 셔츠 | Product isn't returned in search results. | Product is likely returned in search results. |

#### See Also

-   [Enable Data Translation](https://help.salesforce.com/s/articleView?id=commerce.comm_enable_data_translation.htm&language=en_US&type=5 "When you enable data translation, you can translate the data stored in your B2B store product, category, and promotion fields. You can also enable data translation for custom text and URL fields on the product and category objects.")
-   [Manually Localize Product, Category, and Promotion Data](https://help.salesforce.com/s/articleView?id=commerce.comm_create_data_translation.htm&language=en_US&type=5 "You can manually enter translated text for your B2B product and category names and descriptions. To translate promotion names and descriptions, you must use Translation Workbench. To perform bulk translations for product, category, or promotion data, use Translation Workbench.")
-   [Search and Merchandising](https://help.salesforce.com/s/articleView?id=commerce.comm_search_setup.htm&language=en_US&type=5 "Get the most out of your B2B Commerce store by helping shoppers find what they’re looking for.")

Did this article solve your issue?

Let us know so we can improve!

YesNo