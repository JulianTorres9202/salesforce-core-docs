---
title: "Troubleshooting"
source: "https://help.salesforce.com/s/articleView?id=commerce.rt_cms_multilanguage_troubleshooting.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Troubleshooting

Troubleshooting[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Point of Sale](https://help.salesforce.com/s/articleView?id=commerce.rt_intro.htm&language=en_US&type=5)

# Troubleshooting

Make sure that your device's region and language settings are correctly configured to avoid errors while loading a specific app configuration in the Point of Sale CMS Point of Sale (POS) App.

## Cannot find active mobile config for merchant...

If you receive the preceding error message while trying to load a specific app configuration in the POS app, make sure that the device's region and language settings are correctly configured.

## Region

The device's region ‌matches the merchant's region. For example, if the merchant's region in Point of Sale CMS is set to Italy, make sure that the device's region is also set to Italy.

## App Config

The device's language corresponds to the language specified in the app configuration. For instance, if the app configuration is in French, make sure that the device's language is set to French.

## Known Issues and Restrictions

For offline, the deep link is not supported and only the default language that was set will work in offline mode.

If the iPad language is set to a primary language and the store associate prints the receipt in the secondary language, the receipt data, that is, Product Names and reason codes, will only be in the primary language.

Did this article solve your issue?

Let us know so we can improve!

YesNo