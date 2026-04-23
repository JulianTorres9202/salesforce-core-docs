---
title: "Check Numeral System Settings for Locales"
source: "https://help.salesforce.com/s/articleView?id=commerce.b2c_20_6_w7405189_locale_numerals_la.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Check Numeral System Settings for Locales

Check Numeral System Settings for Locales[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2C Commerce Release Notes](https://help.salesforce.com/s/articleView?id=commerce.b2c_parent.htm&language=en_US&type=5)

# Check Numeral System Settings for Locales

Locales now correctly display numbers as defined in Business Manager in the locale's Numeral System setting. Previously, in some cases, the locale used the locale's default Numeral System even though a different Numeral System was configured in Business Manager.

Why: It's possible that some locales that you want to use their default Numeral Systems were configured in Business Manager to use a different Numeral System. Before this fix, this mismatch wasn't a problem because the locales used their default Numeral System anyway. But now locales use the Numeral System configured in Business Manager, which isn’t the one you want.

How: Check your locales to make sure that the Numeral System configured in Business Manager is the one you want to use to display numbers. Go to **Administration** | **Global Preferences** | **Locales**. Click the locale name, and check the **Numeral System** setting under the **General** tab.

Did this article solve your issue?

Let us know so we can improve!

YesNo