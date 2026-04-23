---
title: "Example: Customize a Store Based on a Shopper's Locale"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_ex_markets_customize_based_on_locale.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Example: Customize a Store Based on a Shopper's Locale

Example: Customize a Store Based on a Shopper's Locale[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Example: Customize a Store Based on a Shopper's Locale

Acme Retail is a global fashion retailer that sells to customers in the United States and Europe. Acme can manage an online store in three languages (English, French, and German) by using markets and assigning locales to them. It can also offer different products, prices, promotions, entitlements, and ship-to countries for each market.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

When a shopper selects Germany from the country picker, the website refreshes to show text in German and prices in euros. Because the locale (German | DE) is assigned to the European market, products, pricing, promotions, entitlements, and ship-to countries for the European market are used. If the shopper selects United States, the text switches to English and prices switch to dollars because the locale (United States | EN) is assigned to the United States market. Products sold in and shipped only to countries in the European market are hidden, and pricing and promotions specific to the US market are applied.

#### See Also

-   [Segment a Store into Markets Based on Locale](https://help.salesforce.com/s/articleView?id=commerce.comm_markets.htm&language=en_US&type=5)
-   [Connect REST API Developer Guide: Commerce Webstore Application Context](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_application_context.htm)
-   [Connect REST API Developer Guide: Commerce Webstore Cart Items](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_cart_items)

[](https://help.salesforce.com/s?language=en_US)

## Assign Locales and Ship-To Countries to a Market

This example assumes that you have created your markets and locales, have set up your B2B store’s pricebook, entitlement policies, currencies, and ship-to countries, and have assigned them to the store.

1.  In the navigation sidebar, select the Acme store from the **Store** dropdown.
2.  Select **Settings | Store**, and then click **Markets**.
3.  Select the Alpine Coffee D2C Europe market to assign the French and German locale‌s to it.
4.  Select **Related**.
5.  Next to Locales, select **Assign**, deselect **en\_US**, select **fr** and **de**, and click **Assign**.
6.  Next to Supported Ship-To-Countries, select **Assign**, add France and Germany, and select **Submit**.
7.  In the navigation sidebar, select **Website Design**, and at the bottom left, select the Experience Builder.
8.  In the components palette, drag the Country Selector component to a page in your store. When a customer goes to your store, they can use the Country Selector to select their locale: United States | EN, France | FR, or Germany | DE.
9.  At the top right of the Experience Builder, select **Publish**.

[](https://help.salesforce.com/s?language=en_US)

## Change Shopper’s Locale with Headless API

If you don’t want to use the built-in Country Picker component in your B2B store, you can pass the `language` query parameter directly to the Connect API. All APIs that internally reference entitlements, pricing, promotions, currency, and ship-to countries support the `language` parameter. Here are two examples.

-   [Commerce Webstore Application Context](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_application_context.htm)
-   [Commerce Webstore Cart Items](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_cart_items.htm)

If a store is segmented into markets, these APIs look at the language parameter added to the URL to determine the shopper’s locale and return the appropriate values. In the examples, `language=de` is the German locale for the Alpine Coffee D2C Europe market.

To retrieve the market currency and the ship-to countries that can be used during checkout, use the [Commerce Webstore Application Context](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_application_context.htm) resource API.

```
https://yourInstance.salesforce.com/services/data/v63.0/commerce/webstores/0ZExx0000000001GAA/application-context?language=de
```

To use market-specific pricing and promotions when adding a product to your cart, use the [Commerce Webstore Cart Items](https://developer.salesforce.com/docs/atlas.en-us.chatterapi.meta/chatterapi/connect_resources_commerce_webstore_cart_items.htm) resource API.

```
/commerce/webstores/webstoreId/carts/cartStateOrId/cart-items?language=de
```

Did this article solve your issue?

Let us know so we can improve!

YesNo