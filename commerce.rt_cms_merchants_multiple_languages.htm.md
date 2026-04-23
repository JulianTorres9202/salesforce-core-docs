---
title: "Configuring Merchants with Multiple Languages"
source: "https://help.salesforce.com/s/articleView?id=commerce.rt_cms_merchants_multiple_languages.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Configuring Merchants with Multiple Languages

Configuring Merchants with Multiple Languages[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Point of Sale](https://help.salesforce.com/s/articleView?id=commerce.rt_intro.htm&language=en_US&type=5)

# Configuring Merchants with Multiple Languages

The Point of Sale platform lets you configure merchants based on MerchantID, Locale, and Region.

A merchant on the Point of Sale platform is defined by three values: MerchantID, Locale, and Region. For example, a merchant can be based in the USA, Japan, and Canada.

Merchant ID = a unique merchant ID defined for a merchant.

Region = The country where customers ‌use the Point of Sale app.

Locale = The language within the region.

| MerchantID | Region | Locale |
| --- | --- | --- |
| BrandID | US | en\_US |
| BrandID | JP | ja\_JP |
| BrandID | CA | fr\_CA |

## Localization Components

There are three parts to localization for the POS app

-   App Content
    
    This section refers to all the layouts and app configs for the merchant. The content created in one account can be copied over to other locales. This enables merchants to generate region-specific content in the local language.
    
-   System Buttons, Filters, Icon texts, Date Format
    
    This is bundled with the app binary that is deployed on the device. These are displayed to the user based on their device settings.
    
-   Product Catalog
    
    The product catalog is displayed based on the product feed that the merchant provides the CMS. For a locale of EN (English), you need product details in English and similarly, for FR (French) locale, you need a feed in the French language. This is important as we index different languages separately for effective search and tokenization.
    

## POS Settings

Each locale has different settings based on local regulations, preferences, and hardware configurations. These settings will be defined on CMS under Store, Server, and Active App Config settings. The settings can be copied from one locale to another.

## Promotions

Promotions have different call-out messages, terms, and conditions.

Did this article solve your issue?

Let us know so we can improve!

YesNo