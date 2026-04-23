---
title: "Add a Translate Button to Feed Items in Experience Builder Sites"
source: "https://help.salesforce.com/s/articleView?id=experience.networks_chatter_translate.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Add a Translate Button to Feed Items in Experience Builder Sites

Add a Translate Button to Feed Items in Experience Builder Sites[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Add a Translate Button to Feed Items in Experience Builder Sites

A translation setting in Experience Builder puts a Translate with Google menu on every feed item. Translations are offered through a Google Cloud Translation API key that you provide.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Experience Builder sites accessed through Lightning Experience, Salesforce Classic, and mobile devices, and is available in <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> editions.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To configure feed translations in a site | 
-   Is a System Administrator OR has the permission
-   Manage Experiences OR Create and Set Up Experiences
-   AND is a member of the site

 |

Before you configure translation, go to [https://cloud.google.com/translate](https://cloud.google.com/translate), and get your translation key.

Note Google Cloud Translation is a subscription service. For pricing information, see [https://cloud.google.com/translate/pricing](https://cloud.google.com/translate/pricing).

Take these steps to add a Google Cloud Translation API key to your site.

1.  In Experience Builder, go to **Settings** | **Languages** and enter your Google Cloud Translation API key.
2.  Click **Validate & Save Key**.
    
    This action checks the validity of your key, and, if valid, saves your setting.
    

After you verify and save your key, a **Translate with Google** menu appears on all feed items in your site. Feed items include posts, questions, polls, and their comments, answers, and replies.

-   To translate the feed item into the default language, click **Translate with Google**.
    
    For site members, the default language comes from the locale that’s set on the user’s profile. For guest users, it comes from the locale that’s set in the user’s browser.
    
-   To select a language, click the menu icon and select a language from the list.

These languages appear on the translation list.

<table class="slds-table slds-table_bordered slds-m-bottom_small" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:20%" lwc-3eigj2skqo3=""><col style="width:20%" lwc-3eigj2skqo3=""><col style="width:20%" lwc-3eigj2skqo3=""><col style="width:20%" lwc-3eigj2skqo3=""><col style="width:20%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Albanian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Arabic</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Armenian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Basque</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Bengali</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Bosnian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Bulgarian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Catalan</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Chinese Simplified</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Chinese Traditional</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Croatian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Czech</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Danish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Dutch</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">English</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Estonian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Finnish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">French</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Georgian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">German</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Greek</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Hebrew</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Hindi</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Hungarian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Icelandic</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Indonesian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Irish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Italian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Japanese</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Korean</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Latvian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Lithuanian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Luxembourgish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Macedonian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Malay</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Maltese</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Montenegrin</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Norwegian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Polish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Portuguese</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Romanian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Romansh</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Russian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Serbian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Slovak</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Slovenian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Spanish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Swedish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Tagalog</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Tamil</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Thai</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Turkish</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Ukrainian</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Urdu</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Vietnamese</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Welsh</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">—</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">—</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">—</td><td style="text-align:left;vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">—</td></tr></tbody></table>

After translation, **Translate with Google** switches to **View Original**, so it’s easy to switch back to the original language.

Did this article solve your issue?

Let us know so we can improve!

YesNo