---
title: "What's the Difference Between HML and SML Merge Languages?"
source: "https://help.salesforce.com/s/articleView?id=sales.difference_hml_sml_merge_languages.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# What's the Difference Between HML and SML Merge Languages?

What's the Difference Between HML and SML Merge Languages?[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Seller Productivity](https://help.salesforce.com/s/articleView?id=sales.sales_productivity.htm&language=en_US&type=5)

# What's the Difference Between HML and SML Merge Languages?

Lightning email templates now use the Handlebars Merge Language.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">All</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p style="margin-bottom:0;" lwc-3eigj2skqo3="">List email not available in: <strong lwc-3eigj2skqo3="">Personal</strong>, <strong lwc-3eigj2skqo3="">Contact Manager</strong>, and <strong lwc-3eigj2skqo3="">Group</strong> Editions</p></td></tr></tbody></table>

In Summer ‘18, we introduced the Handlebars Merge Language (HML) for email templates in Lightning Experience. If your email template has merge fields with three curly braces ({{{), you’re using an HML email template. If the merge fields have one curly brace ({), or an exclamation mark (!), you’re using a SML (Salesforce Merge Language) email template. Lightning templates created since Summer ‘18 are HML email templates.

An email template can contain one type of merge field language only.

New abilities include:

-   Recipient merge fields that work with contact lead, and person account records, in one email template
-   ID merge fields that create links to Salesforce records
-   More organization-level fields, such as FY Start Month

#### See Also

-   [Use the Handlebars Merge Language in Lightning Email Templates, Enhanced Letterhead, and Email Template Builder](https://help.salesforce.com/s/articleView?id=sales.handlebars_template_language.htm&language=en_US&type=5 "Use the Handlebars Merge Language—available in Summer ‘18—to add dynamic content to your Lightning and Email Template Builder email templates.")

Did this article solve your issue?

Let us know so we can improve!

YesNo