---
title: "Multi-Language Support"
source: "https://help.salesforce.com/s/articleView?id=service.reply_recs_multi_language.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Multi-Language Support

Multi-Language Support[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [AI Solutions for Service](https://help.salesforce.com/s/articleView?id=service.service_ai_intro.htm&language=en_US&type=5)

# Multi-Language Support

With Einstein Reply Recommendations, you can show service reps common replies in 16 languages during chat and messaging sessions: Arabic, Chinese-simplified, Chinese-traditional, Dutch, English, French, German, Italian, Japanese, Korean, Polish, Portuguese, Russian, Spanish, Thai, and Turkish.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.einstein_service_intro.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To build the Einstein Reply Recommendations model: | Customize Application |

## View and Enable Your Available Languages

Follow the steps in [Set Up Reply Recommendations](https://help.salesforce.com/s/articleView?id=service.reply_rec_set_up.htm&language=en_US&type=5) for Enable Reply Recommendations and Build Your Recommendation Model. Replies are based on a model that Einstein generates by analyzing your closed chat transcripts. Einstein requires at least 1,000 closed chat transcripts per language to deliver replies in that language. If you have insufficient closed chats in all languages or if the chats are too short, you’re alerted when you try to build the model.

Note If you already have a Reply Recommendations model, you must upgrade to the [Hyperforce platform](https://www.salesforce.com/products/platform/hyperforce/). Upgrades will take place on a rolling basis starting June ‘22. During the upgrade Einstein trains and activates a new Reply Recommendations model without any downtime or interruption to service rep experience, and everything works as usual. Along with the retrained model, you receive a new batch of reply templates to review, polish, and publish.

All languages detected by Einstein are listed in the Languages section of the setup page.

The Languages section shows the languages detected (1), the number of transcripts detected in that language (2), whether the model is ready to activate (3), and the model status (4).

To activate a model, select **Disabled/Enabled**. Then follow these steps to [review and publish your replies](https://help.salesforce.com/s/articleView?id=service.reply_rec_publish.htm&language=en_US&type=5).

Did this article solve your issue?

Let us know so we can improve!

YesNo