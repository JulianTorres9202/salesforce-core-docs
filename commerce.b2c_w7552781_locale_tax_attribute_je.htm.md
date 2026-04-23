---
title: "Localize Product Tax Classes with the Localized Tax Class ID Attribute"
source: "https://help.salesforce.com/s/articleView?id=commerce.b2c_w7552781_locale_tax_attribute_je.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Localize Product Tax Classes with the Localized Tax Class ID Attribute

Localize Product Tax Classes with the Localized Tax Class ID Attribute[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2C Commerce Release Notes](https://help.salesforce.com/s/articleView?id=commerce.b2c_parent.htm&language=en_US&type=5)

# Localize Product Tax Classes with the Localized Tax Class ID Attribute

If you operate one site across multiple regions, you can use the localizedTaxClassId to define different tax class Ids for the same product in different locales. The new attribute eliminates the need to map a different tax rate for each product that requires a specific tax handling.

How: The attribute is a global product preference. To change your system preference to use the localizedTaxClassId, in Business Manager, select **Administration** | **Global Preferences** | **Products**. Check Localized Tax Class for Product. The taxClassId is the default for SFRA and SiteGenesis sites.

Note The taxClassId attribute is not changed or deprecated. You can provide values for both attributes, but only the active attribute is used.

Did this article solve your issue?

Let us know so we can improve!

YesNo