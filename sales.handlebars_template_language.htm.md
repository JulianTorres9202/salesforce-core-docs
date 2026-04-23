---
title: "Use the Handlebars Merge Language in Lightning Email Templates, Enhanced Letterhead, and Email Template Builder"
source: "https://help.salesforce.com/s/articleView?id=sales.handlebars_template_language.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "sales"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Use the Handlebars Merge Language in Lightning Email Templates, Enhanced Letterhead, and Email Template Builder

Use the Handlebars Merge Language in Lightning Email Templates, Enhanced Letterhead, and Email Template Builder[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Seller Productivity](https://help.salesforce.com/s/articleView?id=sales.sales_productivity.htm&language=en_US&type=5)

# Use the Handlebars Merge Language in Lightning Email Templates, Enhanced Letterhead, and Email Template Builder

Use the Handlebars Merge Language—available in Summer ‘18—to add dynamic content to your Lightning and Email Template Builder email templates.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Lightning Email Templates are available in: Lightning Experience</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">All</strong> Editions</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><p style="margin-bottom:0;" lwc-3eigj2skqo3="">List email not available in: <strong lwc-3eigj2skqo3="">Personal</strong>, <strong lwc-3eigj2skqo3="">Contact Manager</strong>, and <strong lwc-3eigj2skqo3="">Group</strong> Editions</p></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">&nbsp;</td></tr></tbody></table>

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience for email templates created in Email Template Builder and Email Content Builder</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: <strong lwc-3eigj2skqo3="">Professional</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions.</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Account Engagement Lightning App for all Account Engagement editions</td></tr></tbody></table>

Note

In Summer ‘18, we introduced the Handlebars Merge Language (HML) for email templates in Lightning Experience. If your email template has merge fields with three curly braces ({{{), you’re using an HML email template. If the merge fields have one curly brace ({), or an exclamation mark (!), you’re using a SML (Salesforce Merge Language) email template. Lightning templates created since Summer ‘18 are HML email templates.

Although based on the Handlebars template language, our HML implementation doesn’t contain every Handlebars feature.

New ways to use merge fields include:

-   Recipient merge fields that work with contact, lead, and person account records, in one email template
    
    Note
    
    Not every merge field can be used with every email recipient. For example, the {{{Recipient.Department}}} merge field can be used with contacts only, while no recipient merge fields can be used when a user is the recipient.
    
    The Insert Merge Field window shows you which fields work with both Lead and Contact (1), with Contact only (2), or with Lead only (3).
    
-   ID merge fields that create links to Salesforce records
-   More organization-level fields, such as FY Start Month

Email templates using HML can be used in list emails.

## Guidelines for Syntax and Formatting

The syntax consists of three open curly braces, followed by the object name, a period, the field name, and three closing curly braces.

For example, to include your recipient’s first name, the merge field is {{{Recipient.FirstName}}}. If you want to include the account ID number of the account related to the email, enter or choose this merge field: {{{Account.Id}}}. When you preview or send the email, ID: 001234567890123 displays where you inserted the merge field.

[](https://help.salesforce.com/s?language=en_US)If two or more custom objects have matching names or labels, only one of the objects appears when you select from available merge fields. Make sure that all custom objects have unique names and labels so that you can select merge fields from any of the objects.

[](https://help.salesforce.com/s?language=en_US)To make sure you’re using the correct syntax, select merge fields from the merge field picker.

Tip Most merge fields for email templates correspond directly with email template fields. If there’s a merge field you want to use that’s not listed in the picker, type it as plain text.

To use the merge field {{{Sender.Signature}}}, have users set up their signature in My Email Settings.

Note In the merge picker, the merge field is listed as Email Signature.

#### See Also

-   [Convert a Lightning Email Template from SML to HML](https://help.salesforce.com/s/articleView?id=sales.email_template_convert_from_sml_to_hml.htm&language=en_US&type=5 "Take advantage of the Handlebars Merge Language (HML), which is more flexible than the Salesforce Merge Language (SML), by converting existing Lightning email templates.")
-   [Considerations for Using Merge Fields in Email Templates and Letterheads](https://help.salesforce.com/s/articleView?id=sales.merge_fields_email_templates.htm&language=en_US&type=5 "A merge field is a placeholder used in an email, a letterhead, a mail merge template, a custom link, or a formula to incorporate values from a record. When you send the email, the placeholder is replaced with the data from the record or records of the people you’re emailing.")

Did this article solve your issue?

Let us know so we can improve!

YesNo