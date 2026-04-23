---
title: "Specify a Date Format for Locales"
source: "https://help.salesforce.com/s/articleView?id=commerce.b2c_rn_specify_date_format_for_locales.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Specify a Date Format for Locales

Specify a Date Format for Locales[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2C Commerce Release Notes](https://help.salesforce.com/s/articleView?id=commerce.b2c_parent.htm&language=en_US&type=5)

# Specify a Date Format for Locales

You can now modify the date settings format in Business Manager so that the script API method `dw.util.Calendar.getFirstDayOfWeek()` returns the first day of the week in the date format used by your site locale. Previously, you couldn’t modify the date format to match the local or regional context.

**How:** You configure the date setting format in **Business Manager** | **Administration** | **Global Preferences** | **Locales**. For your locale, select the Regional Settings and modify the Date Settings. The date setting format affects Business Manager related Date Picker interfaces. The setting also sets the date format of the returned date value for the Script API method `dw.util.Calendar.getFirstDayOfWeek()`.

#### See Also

-   [Configure Site Locales for B2C Commerce](https://help.salesforce.com/s/articleView?id=cc.b2c_configuring_site_locales.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo