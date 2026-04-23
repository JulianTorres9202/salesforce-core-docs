---
title: "Translate Messaging Components into Your Customer’s Language"
source: "https://help.salesforce.com/s/articleView?id=service.messaging_components_translate.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "service"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Translate Messaging Components into Your Customer’s Language

Translate Messaging Components into Your Customer’s Language[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Agentforce Contact Center](https://help.salesforce.com/s/articleView?id=service.support_channels.htm&language=en_US&type=5)

# Translate Messaging Components into Your Customer’s Language

Show messaging components in a customer’s preferred language with the help of Translation Workbench. For example, when you send a French-speaking customer a question with three options, show the question and options translated into French.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""><col style="width:50%" lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" colspan="2" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=service.messaging_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions.</a></td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a name="messaging_components_translate__d828e834" lwc-3eigj2skqo3="" href="https://help.salesforce.com/s?language=en_US"></a><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="Checkmark" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/checkmark.png" id="messaging_components_translate__d828e834" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article applies to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Enhanced In-App Chat, Enhanced Web Chat v1, Enhanced Web Chat v2, Enhanced WhatsApp, Enhanced Facebook Messenger, Enhanced Apple Messages for Business, Enhanced LINE, and Bring Your Own Channel</td></tr><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><span style="vertical-align:text-bottom;display:inline-block;" lwc-3eigj2skqo3=""><img alt="X icon" src="https://sf-zdocs-cdn-prod.zoominsoftware.com/tdta-support_channels-260-0-0-production-enus/e42a3c30-73dc-4e82-8320-0ade019503d6/resources-global/_corporate/images/crossmark.png" style="margin-bottom:0;" lwc-3eigj2skqo3=""></span> <strong lwc-3eigj2skqo3="">This article doesn’t apply to:</strong></td><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Standard Facebook Messenger, and Standard and Enhanced SMS channels</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To create messaging components: | 
Customize Application AND View Setup and Configuration

OR

System Administrator

 |
| To send and receive messages in Messaging: | Messaging Agent |
| To import and export translation files: | Manage Translation AND Customize Application |

Note Automated messaging doesn’t yet support translated messaging components. If you’re using a flow to automatically send notification messaging components, the original, untranslated version of the component is sent to customers.

#### See Also

-   [Enable or Disable Translation Workbench](https://help.salesforce.com/s/articleView?id=platform.customize_wbench.htm&language=en_US&type=5)
-   [Add Translated Languages and Translators](https://help.salesforce.com/s/articleView?id=platform.adding_and_editing_translated_languages.htm&language=en_US&type=5)
-   [Export Data Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export_data.htm&language=en_US&type=5)
-   [Import Translated Files](https://help.salesforce.com/s/articleView?id=platform.workbench_import.htm&language=en_US&type=5)
-   [Configure Field-Level Security](https://help.salesforce.com/s/articleView?id=ind.fsc_admin_configure_field_level_security.htm&language=en_US&type=5)

[](https://help.salesforce.com/s?language=en_US)

## Step 1: Set Up Translation Workbench

To get started, enable Translation Workbench and select your languages.

1.  Enable Translation Workbench in Setup.
2.  Add one or more languages. For example, if your default org language is English but you want messaging components to be available in French and Spanish, add French and Spanish.

[](https://help.salesforce.com/s?language=en_US)

## Step 2: Prepare Your Messaging Components for Translation

Two parts of a messaging component can be translated:

-   The component name, which service reps see in the Service Console.
-   All constant values, which are managed from the Constants tab in the Messaging Component Builder. Constants determine the text in the messaging component that customers receive in a message. Several standard constants are automatically added when you first create a component. You can also add custom constants.

If any text in a messaging component is literal, rather than determined by a constant, it can’t be translated and remains in the default org language. To verify that a messaging component uses constants for all text that you want translated, create or open the component in the Messaging Component Builder.

1.  In Setup, go to the Messaging Components page.
2.  Click the name of the messaging component that you want to be translated.
3.  In the left-hand sidebar, click the **Text** format.
4.  In the properties pane, review each Formula Template field. If the formula template contains literal text instead of constants, create a custom constant that can replace the literal text. For example, in this question with options component, a constant must replace the phrase “Select an option” in the first formula template so it can be translated.
    1.  In the left-hand sidebar, click **Constants**.
    2.  Click **New**.
    3.  Give your constant a name, such as SelectionPrompt, and save it.
    4.  Click the Text format again.
    5.  In the formula template, replace the literal text with your constant. In this example, Select an option becomes {!$Constants.SelectionPrompt}.
    6.  Save your changes.
5.  If another format was added, click the format name in the left-hand sidebar.
6.  In the properties pane, verify that the Type field for all text to be translated is set to Constant and that a constant is selected in the field after it. In this example, the Quick Replies format on a question with static options component is correctly configured.
7.  After you configure the properties of all formats added to your component, save your changes.

Note Some text in a messaging component doesn’t need to be translated, such as URLs. This text can stay as literal text in a formula template or component property.

[](https://help.salesforce.com/s?language=en_US)

## Step 3: Translate Your Component Text

To provide translated versions of a messaging component, manually enter the translation or import a batch of translated text. If you plan to translate multiple messaging components or translate to multiple languages, importing is faster.

[](https://help.salesforce.com/s?language=en_US)Important A messaging component is translated only if Translation Workbench contains translations of all of the component's text constants. For example, if your component includes three constants, provide translations of all three constants. If a translation of any constant is missing, the component isn't translated. This rule helps service reps avoid sending a message that uses multiple languages.

Provide translations manually:

1.  In Setup, go to the Translate page under Translation Workbench.
2.  In the Language field, select the language to which you want to translate your messaging component; for example, French.
3.  In the Setup Component field, select **Messaging Component**.
4.  In the Messaging Component field, select the developer name of the component to be translated.
5.  In the Object field, select **Messaging Component Name**. The component name appears in a table.
6.  Hover over the table and click the pencil icon, then enter the translation of the messaging component name. For example, service reps whose language is set to French see the French name of the component in the Service Console.
7.  In the Object field, select Constant Values. All of the component’s constants appear in a table.
8.  Hover over the table and click the pencil icon, then enter the translation of each constant.
9.  Save your changes.

To provide translations in a batch, export a data translation file from the Export page in Setup under Translation Workbench. When exporting, select the Messaging Component Name or Constant Values object. After completing one file per language, import them on the Import page.

[](https://help.salesforce.com/s?language=en_US)

## Step 4: Send Translated Messaging Components

After you provide translated versions of your messaging components, your support team can send them to customers.

Note For enhanced chat, enhanced Apple Messages for Business and Bring Your Own Channels, you can now enable the **Identify preferred language of messaging users** option in Setup, so Salesforce auto-populates the Language field.

1.  (Admin task) Enable access to the Messaging User Language field for service rep profiles, and then add it to the Messaging Session page layout. Service reps need edit access to this field to send translated messaging components.
2.  At the start of a messaging session, update the Messaging User Language field on the messaging session record to list the customer’s preferred language. You can gather this information contextually or via a bot question that auto-completes the field.
    
    If you enabled the **Identify preferred language of messaging users** option in Setup, you can skip this step.
    
3.  Click the messaging component action and click **Insert** on a component to send.
4.  Click **Send**. If Translation Workbench contains a version of the component in the customer’s preferred language, the customer sees the messaging component in their language. 

Example Your default org language is English, and you created a range of messaging components in English. To support your French-speaking customers, you upload French translations of the components in Translation Workbench.

When a customer initiates a messaging session with a French message, the service rep updates the Messaging User Language on the session record to French. Any components that the rep sends during the session appear to the customer in French. 

If a component is available in a service rep's default language, the rep sees the component name in their language in the list of messaging components shown in the Service Console. Otherwise, it shows the original component name.

[](https://help.salesforce.com/s?language=en_US)Note While auto-response messaging components can be translated like any other component, the messaging session record must list a Messaging User Language so Salesforce knows what language to use. Auto-response messaging components aren't translated for Enhanced WhatsApp, Enhanced Facebook Messenger, Enhanced SMS, and Enhanced LINE channels.

[](https://help.salesforce.com/s?language=en_US)

## Step 5: Keep Translations Up to Date

If a messaging component is updated in the Messaging Component Builder, it’s important to update translations of the component to reflect the changes. Regularly check for outdated translations and update them as needed.

On the Translate page in Setup, **Out of date** is selected on any translations whose original language underwent an update after the translated version was saved. You can manually update individual translations on the Translate page. Or, go to the Export page and export a list of messaging component translations marked **Out of date**.

Did this article solve your issue?

Let us know so we can improve!

YesNo