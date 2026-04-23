---
title: "Translate Service Documents in Document Builder"
source: "https://help.salesforce.com/s/articleView?id=service.fs_document_builder_translate.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Service Documents in Document Builder

Translate Service Documents in Document Builder[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Salesforce Field Service](https://help.salesforce.com/s/articleView?id=service.fs_overview.htm&language=en_US&type=5)

# Translate Service Documents in Document Builder

With Document Builder, translate service documents into any language supported by the Salesforce platform. Specify different languages for different records to translate the document to the preferred language of individual customers.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Lightning Experience.</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">The Field Service core features, managed package, and mobile app are available in <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> Editions.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To create service documents with Document Builder: | Field Service Document Builder Dispatcher, Field Service Document Builder Mobile, OR Field Service Document Builder Standard permission sets |

1.  From Setup, enter Translation Workbench in the Quick Find box, and then select **Translation Language Settings**.
2.  Enable Translation Workbench
3.  To add a language, select **Add**.
4.  Select the languages you want to support for each user from the dropdown list and identify which users you want to be able to translate using those languages.
5.  From the Object Manager in Setup, select **Work Order**.
    
    Note Languages are set on work orders only. All service appointments under a work order are translated into the same language.
    
6.  In the Page Layouts section, add the Service Report Language field. The languages you chose in Translation Workbench are shown in the Service Report Language field’s dropdown list.
7.  When generating a service document with Document Builder, select your preferred language from the Service Report Language field.

To test service document translation, generate a service document from the work order or a child service appointment. When you preview the PDF, the service document is translated into the language you selected.

#### See Also

-   [Generate Service Document PDFs on the Desktop Site](https://help.salesforce.com/s/articleView?id=service.fs_generate_pdfs_desktop.htm&language=en_US&type=5 "With Document Builder, you can generate PDFs from the desktop site and mobile app. This topic walks you through the process for the desktop site.")
-   [Generate Service Document PDFs on the Mobile App](https://help.salesforce.com/s/articleView?id=service.fs_generate_pdfs_mobile.htm&language=en_US&type=5 "With Document Builder, you can generate PDFs from the desktop site and mobile app. This topic walks you through the process for the Field Service mobile app.")

Did this article solve your issue?

Let us know so we can improve!

YesNo