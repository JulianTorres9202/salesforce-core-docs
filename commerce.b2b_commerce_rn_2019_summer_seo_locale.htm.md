---
title: "Add SEO Support for All Regions and Languages"
source: "https://help.salesforce.com/s/articleView?id=commerce.b2b_commerce_rn_2019_summer_seo_locale.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Add SEO Support for All Regions and Languages

Add SEO Support for All Regions and Languages[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce for Visualforce](https://help.salesforce.com/s/articleView?id=commerce.b2b_commerce_release_notes.htm&language=en_US&type=5)

# Add SEO Support for All Regions and Languages

Make it easier for search engine bots to crawl and index your localized Home page, Product List page, and Product Detail page. B2B Commerce for Visualforce now complements the default-locale canonical link in a page’s `<head>` with locale-specific alternate links. With this change, search engines can show your localized page content in search results for the languages and regions your storefront supports.

**Where:** This change applies to **B2B Commerce for Visualforce Summer ’19 (version 4.11)** in Lightning Experience and Salesforce Classic in Enterprise, Performance, Unlimited, and Developer editions.

**Who:** This metadata is included on the Home page, Product List page, and Product Detail page for guest users, including bots. B2B Commerce for Visualforce already serves localized content to authenticated storefront users based on their locale.

**Why:** Previous versions of B2B Commerce for Visualforce included a canonical link in the `<head>` of the Home, Product List, and Product Detail pages. Because the canonical link value didn’t include any language-specific information, the canonical link always resolved to content in the storefront’s default language.

With this change, you can better support the external search experience of your target locales. For example, if your storefront supports Japanese, you can make sure that search engines index the Japanese versions of your pages. Then, a user in Japan can find search results from your storefront in Japanese.

**How:** After you upgrade the available global data, a new storefront configuration setting, Enable Canonical and Alternate Language Links, is available under the User Interface module. By default, this setting is FALSE. To start inserting alternate language links, change this setting to TRUE.

After you enable the configuration setting, the following `<link>` metadata is inserted:

-   A `<link rel="canonical" href="canonicalURL?cclcl="guestUserLocale">` element for the page's canonical URL and storefront guest user's locale
-   A `<link rel="alternate" hreflang="guestUserLocale" href="canonicalURL?cclcl="guestUserLocale">` element for the storefront guest user's locale
-   A `<link rel="alternate" hreflang="anotherLocale" href="canonicalURL?cclcl="anotherLocale">` element for each additional language that your storefront supports

Note Sitemaps include your canonical URLs, but don't include any alternate language links.

For more details, check out the help for alternate language links in your storefront pages.

The `ccrz.cc_hk_UserInterface.canonicalUrlInclude()` method supports this change. Previously, this method returned only the URL value for a page’s canonical URL. Now, this method returns the URL values for a page’s canonical URL and alternative language links for any selected storefront languages. If you previously created subscriber code to extend this method, update your code to account for the new returned information, if necessary.

Did this article solve your issue?

Let us know so we can improve!

YesNo