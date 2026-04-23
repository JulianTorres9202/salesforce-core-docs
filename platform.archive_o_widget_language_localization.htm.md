---
title: "Archive Widget Language Localization"
source: "https://help.salesforce.com/s/articleView?id=platform.archive_o_widget_language_localization.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "platform"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Archive Widget Language Localization

Archive Widget Language Localization[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Own from Salesforce](https://help.salesforce.com/s/articleView?id=platform.own_from_salesforce.htm&language=en_US&type=5)

# Archive Widget Language Localization

Translate Archive Widget into the local language of your end users in the Archive managed package.

Note This content relates to Archive. For Salesforce Archive, see [Store Data Externally with Salesforce Archive](https://help.salesforce.com/s/articleView?id=xcloud.archive_overview.htm&language=en_US&type=5).

This feature is supported in Package 17 and later.

To set up your org for translation, see [Add Translated Languages and Translators](https://help.salesforce.com/s/articleView?id=platform.adding_and_editing_translated_languages.htm&language=en_US&type=5%3B).

Translation is done via Custom Labels. For more information, see [Translate Custom Labels.](https://help.salesforce.com/s/articleView?id=platform.cl_translate_edit.htm&language=en_US&type=5)

To translate Archive Widget:

1.  Go to Setup.
2.  Search for Custom Labels in Quick Search.
    
    All archive-related labels have a prefix of `Archive_`.
    
3.  Click the custom label to be translated.
4.  Click **New Local Translations/Overrides**.
5.  From the Translation Information dropdown list, select the required language.
6.  Click **Save**.

Available Custom Labels
| Custom Label Name | Description | Default Archive Label |
| --- | --- | --- |
| Archived\_Record\_Link | Link references the archive parent record. The `(Archived)` concatenated. | Archived |
| Archive\_Back\_To\_Search\_Results | Link on the widget and global search. | Back to Search Results |
| Archive\_Change\_Selected\_Filters\_Message | Second line when there are no results, suggested actions. | The widget searches for a second line message when there are no results, suggesting recommended actions. |
| Archive\_Export\_Started\_Message | Pop-up message when an export process starts. | Export Started |
| Archive\_No\_Results\_Message | Widget search main message when there are no results. | No Result Found |
| Archive\_Show\_More\_Results\_Button | Button that displays below the widget when the widget has more results. | Show More Results |
| Archive\_Unarchive\_Started\_Message | Pop-up message when an unarchive process starts. | Unarchive Started |
| Archive\_Widget\_Archive\_Records\_Title | Title in the archive widget of the archived records. | Archived Records |
| Archive\_Widget\_Global\_Detail | Detail tab name of the archived record. | Detail |
| Archive\_Widget\_Global\_Download\_Action | Label for the action and button of download. | Download |
| Archive\_Widget\_Global\_Export\_Action | Label for the action and button of export. | Export |
| Archive\_Widget\_Global\_Found\_result\_Summary | Header is in the exact format: Page "{0}" out of "{1}" - about "{2}" results | Page {0} out of {1} - about {2} results |
| Archive\_Widget\_Global\_Preview\_Action | Label for the action and button of preview. | Preview |
| Archive\_Widget\_Global\_Related | Related tab name of the archived record. | Related |
| Archive\_Widget\_Global\_Related\_Legal\_Hold | Related tab name of the archived record. | Related Legal Hold Requests |
| Archive\_Widget\_Global\_Unarchive\_Action | Label for the action and button of unarchive. | Unarchive |
| Archive\_Widget\_Global\_View\_Action | Action of view record. | View |
| Archive\_Widget\_Select\_Objects | Dropdown hint text of the object search on the widget. | Select Object |

Examples for Archive Widget in French, according to this table.

| Custom Label | French Translation |
| --- | --- |
| Archive\_Back\_To\_Search\_Results | Retour sur les résultats de la recherche |
| Archive\_Change\_Selected\_Filters\_Message | Veuillez recommencer votre recherche |
| Archive\_Export\_Started\_Message | Le processus d'exportation a été initié |
| Archive\_No\_Results\_Message | Aucun résultat |
| Archive\_Unarchive\_Started\_Message | Le processus de désarchivage a été initié |
| Archive\_Widget\_Archive\_Records\_Title | Données archivées |
| Archive\_Widget\_Global\_Detail | Détails |
| Archive\_Widget\_Global\_Download\_Action | Télécharger |
| Archive\_Widget\_Global\_Export\_Action | Exporter |
| Archive\_Widget\_Global\_Found\_result\_Summary | Page {0}/{1} - sur {2} résultats |
| Archive\_Widget\_Global\_Preview\_Action | Aperçu |
| Archive\_Widget\_Global\_Related | Données Reliées |
| Archive\_Widget\_Global\_Related\_Legal\_Hold |   |
| Archive\_Widget\_Global\_Unarchive\_Action | Désarchiver |
| Archive\_Widget\_Global\_View\_Action | Voir |
| Archive\_Widget\_Select\_Objects | Sélectionner |
| Archived\_Record\_Link | Archivé |

Did this article solve your issue?

Let us know so we can improve!

YesNo