---
title: "Multiple Language Configuration on Point of Sale CMS"
source: "https://help.salesforce.com/s/articleView?id=commerce.rt_cms_multiple_language_configuration.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Multiple Language Configuration on Point of Sale CMS

Multiple Language Configuration on Point of Sale CMS[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Point of Sale](https://help.salesforce.com/s/articleView?id=commerce.rt_intro.htm&language=en_US&type=5)

# Multiple Language Configuration on Point of Sale CMS

Point of Sale CMS lets you set up POS apps in different languages. You can also set up email and print templates, layouts, promotions, reason codes, and tax.

## POS App Configuration

The sections that are supported with the multilanguage feature are pos app configs, email & print templates, layouts, promotions, reason codes, and tax. Products are also supported, however, the multilanguage feature is configured through the feed.

To view a list of POS app configurations that are configured to a specific language:

1.  Go to **CMS > Apps > All**.
2.  Select the language using the Language dropdown in the upper left of the screen.

Important Currently, changing the language of a specific app configuration has been disabled.

## Email & Print Templates

To view a list of email & print templates that are configured to a specific language:

1.  Go to **CMS > Store Management > Email & Print Templates.**
2.  Select the language using the **Language** dropdown.

To change the language of an email & print template:

1.  Go to **CMS > Store Management > Email & Print Templates > your template > Edit**.
2.  Select the language using the **Language** dropdown.
3.  Click **PUBLISH**.

## Layouts

To view a list of layouts that are configured for a specific language:

1.  Go to **CMS > Layouts > All Layouts**.
2.  Select the language using the **Language** dropdown.

Important Currently, changing the language of a specific layout has been disabled.

## Promotions

When you create a promotion, it is applicable across all languages within the same region. This means that there's one promotion with a single promo code, but it can have separate names, titles, and descriptions for each language. If you need different promo codes for different regions, create separate promotions for each region.

Always configure the promotion in the default language (also known as the base language) otherwise, you receive an error indicating so. Additionally, the redemption rate will be shared across as the promotion is essentially the same but associated with a different language.

To view a list of promotions that are configured for a specific language:

1.  Go to **CMS > Promotions**.
2.  Select the language using the **Language** dropdown.

To change the language of a promotion:

1.  Go to **CMS > Promotions**.
2.  Select a promotion by clicking on the pencil icon to the right of it.
3.  Select the language using the **Language** dropdown in the upper left of the screen.
4.  Select **PUBLISH NOW** or **Schedule**.

## Reason Codes

To view a list of reason codes that are configured for a specific language:

1.  Go to **CMS > Store Management > Reason Codes**.
2.  Select the language using the **Language** dropdown.

## Tax

The tax rates behave similarly to the products in which it uses a feed to show the information for a certain locale. For more information, see [Product Feeds for Multiple Languages](https://help.salesforce.com/s/articleView?id=commerce.rt_cms_product_feeds.htm&language=en_US&type=5 "Use product feeds in Point of Sale CMS to manage products in multiple languages.").

To view a list of tax rates that are configured to a specific language:

1.  Go to **CMS > Store Management > Tax > View Tax Rates**.
2.  Select the language using the **Language** dropdown.

To view a list of tax exemptions that are configured to a specific language:

1.  Go to **CMS > Store Management > Tax > Tax Exemption Configuration**.
2.  Select the language using the **Language** dropdown.

Did this article solve your issue?

Let us know so we can improve!

YesNo