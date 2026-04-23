---
title: "Export Language Content"
source: "https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_export.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Export Language Content

Export Language Content[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Export Language Content

Export and prepare Experience Builder site content as one or multiple .xml files. Prepare the files for translation by creating nodes for specific languages. Then send the file to your translation service.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3="">Available in: Experience Builder sites accessed through Lightning Experience, Salesforce Classic, and mobile devices, and is available in <strong lwc-3eigj2skqo3="">Essentials</strong>, <strong lwc-3eigj2skqo3="">Enterprise</strong>, <strong lwc-3eigj2skqo3="">Performance</strong>, <strong lwc-3eigj2skqo3="">Unlimited</strong>, and <strong lwc-3eigj2skqo3="">Developer</strong> editions.</td></tr></tbody></table>

| User Permissions Needed |
| --- |
| To customize or publish an Experience Cloud site: | 
-   Create and Set Up Experiences AND View Setup and Configuration AND be a member of the site
    
    OR
    
-   View Setup and Configuration AND be a member of the site AND have appropriate [role-based site access](https://help.salesforce.com/s/articleView?id=experience.networks_access_control_overview.htm&language=en_US&type=5)

 |

Before you begin, let’s look at the structure of the .xml file that’s created when you export language content. The file consists of several elements, and these elements are the key ones to focus on.

-   `component` elements represent the page components that make up your site. Many of these components contain text that must be translated.
-   The `field` element contains the component’s properties for a particular language. The language is defined by the `language` attribute.
-   `property` elements include `CDATA` tags that contain the text strings for translation.
    
    As you can see in this sample XML for a component, several `CDATA` tags don’t contain any content. So the only `CDATA` tags that you and your translators must focus on are the ones that contain text.
    

```markup
<component context="Contact Support Form (Aura)" documentId="2342fd59-55da-5bdd-b013-d0a3cb6ce523" id="1242fd59-76da-4cdd-b025-d0a3cb6ce496">
    <field name="AuraAttributes" language="en_US" exportcrc="811168867">
        <property name="requestSummaryText"><![CDATA[Case summary]]></property>
        <property name="callToActionText"><![CDATA[]]></property>
        <property name="headerSubtitle"><![CDATA[Tell us how we can help.]]></property>
        <property name="callToActionButtonText"><![CDATA[]]></property>
        <property name="confirmationText"><![CDATA[Your case was created.]]></property>
        <property name="confirmationSubtext"><![CDATA[We'll get back to you soon.]]></property>
        <property name="headerTitle"><![CDATA[Contact Customer Support]]></property>
    </field>
</component>
```

Note If you exported your site content for translation before Winter ’22, you can’t import the resulting translated file. To ensure a successful import, export your site content again and translate it in this more recent .xml file.

To export and prepare content for translation:

1.  In Experience Builder, click  | **Languages**.
2.  Click **Export Content**.
3.  Select your default language.
    
    You can select a language other than your default language, but we don’t recommend it unless you must export existing translations for that particular language. If you haven’t yet added translations for the language, the exported file is empty.
    
4.  (Optional) Change the export file name.
    
    The default name of this file is Languages.xml, but you can rename it. Consider exporting a file for each translation and renaming each file by its country code. For example, if you intend to get translations for French, German, and Spanish, you can rename the files language\_fr.xml, language\_de.xml, and language\_es\_mx.xml, respectively.
    
5.  Click **Export**.
6.  If you’re prompted to, choose where to save the file.
7.  Prepare the .xml file for translation.
    1.  Copy the `field` element for the content to be translated, and paste the copy under the original.
        
        You can copy a `field` element multiple times for multiple translations in one file. However, to reduce the chance of overwriting existing translations when importing new ones, we recommend that you export a separate Languages.xml file for each translation.
        
    2.  Update the `language` attribute in the pasted `field` element to the new language.
    3.  Save your changes.

After you export and prepare the .xml file, you can send it for translation. Ask your translators to put translated content between the brackets that follow the `CDATA` tags.

If possible, avoid updating the site’s default content until after you receive and import your translated content. Because the translated file contains the original default content and the translated content, when you import the file, you overwrite updates made in the interim.

Note Keep this consideration in mind for translations when you make a new property of a custom component available for edit in Experience Builder: If the component is in use on a page in Experience Builder, delete the component from the page and replace it with the updated version. Otherwise, when you export the site content for translation, the property that you added is omitted for that component instance in the exported file. If the component contains content that’s already translated, export the site content first to preserve the existing translation. Then replace the component with the updated version. For more information, see [Aura Component Bundle Design Resources](https://developer.salesforce.com/docs/atlas.en-us.lightning.meta/lightning/components_config_for_app_builder_design_files.htm) or, for Lightning web components, [Configure a Component for Experience Builder](https://developer.salesforce.com/docs/component-library/documentation/en/lwc/use_config_for_community_builder).

When you receive the translated .xml file, [import it back into the site.](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_import.htm&language=en_US&type=5 "After your translation service has completed the translations, import the translated .xml file into your Experience Builder site.")

#### See Also

-   [Import Translated Content](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_import.htm&language=en_US&type=5 "After your translation service has completed the translations, import the translated .xml file into your Experience Builder site.")

Did this article solve your issue?

Let us know so we can improve!

YesNo