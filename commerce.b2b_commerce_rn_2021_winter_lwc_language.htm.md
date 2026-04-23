---
title: "Support Experience Builder Site Languages with the Locale Switcher Widget"
source: "https://help.salesforce.com/s/articleView?id=commerce.b2b_commerce_rn_2021_winter_lwc_language.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Support Experience Builder Site Languages with the Locale Switcher Widget

Support Experience Builder Site Languages with the Locale Switcher Widget[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce for Visualforce](https://help.salesforce.com/s/articleView?id=commerce.b2b_commerce_release_notes.htm&language=en_US&type=5)

# Support Experience Builder Site Languages with the Locale Switcher Widget

If your storefront supports multiple locales, you can support the corresponding language from the Locale Switcher widget in the B2B Commerce Header component for an Experience Builder site.

**Where:** This change applies to **B2B Commerce for Visualforce Winter ’21 (version 4.13)** in Lightning Experience and Salesforce Classic in Enterprise, Performance, Unlimited, and Developer editions.

**Why:** In previous versions of B2B Commerce for Visualforce, the B2B Commerce Header component for an Experience Builder site didn't show the Locale Switcher widget at all.

This release adds the Locale Switcher widget to the B2B Commerce Header component, which provides parity with the standard header component for a Visualforce storefront page. However, an Experience Builder site and the B2B Commerce for Visualforce managed package support language internationalization differently:

-   An Experience Builder site supports its own set of languages, and uses the language URL parameter to specify the current language.
-   The B2B Commerce for Visualforce managed package supports its own set of locales, with a language assigned to each locale. A Visualforce storefront page uses the cclcl parameter to specify the current locale, which determines the current language.

Tip We recommend that you manually enable the same languages and locales for both your Experience Builder site and Visualforce storefront. B2B Commerce doesn't provide an option for automatically synchronizing these settings, and the managed package potentially supports more languages than Experience Builder. To support a language consistently across both Experience Builder and Visualforce pages, the language must match exactly.

**How:** After you upgrade the managed package, the new B2B Commerce Header component includes the Locale Switcher widget automatically.

When a registered buyer or guest buyer changes their selected locale, the language and cclcl parameters stay synchronized. As the buyer navigates between Experience Builder site pages and the Visualforce storefront, the buyer's selected language persists across experiences.

The following changes in the managed package's default data sets support this enhancement:

-   In the default global data (the CC\_Data\_Global static resource), the Locale Switcher storefront configuration module's Enabled setting (`ls.enabled`) now has the Externally Safe option set to TRUE. Update the metadata for this configuration.
-   In the Capricorn Coffee demo storefront data (the CC\_Data\_DefaultStore static resource), all records internationalized for Japanese have been updated to use the `ja` locale instead of the `ja_JP` locale. This change ensures that the internationalized demo data displays correctly on an Experience Builder site page when a buyer selects Japanese.

Did this article solve your issue?

Let us know so we can improve!

YesNo