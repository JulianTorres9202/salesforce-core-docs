---
title: "Structure of the Store Metadata Translation Source File"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_metadata_translation_source_file.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Structure of the Store Metadata Translation Source File

Structure of the Store Metadata Translation Source File[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Structure of the Store Metadata Translation Source File

In situations where Salesforce doesn’t provide default metadata translations, you can localize your store’s metadata and the custom functionality that you build.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

The metadata XLIFF source file, that you download from the Translation Workbench, includes all of your store’s translatable metadata. The file’s element structure is specific to your store.

## Metadate Translation Source File Syntax

The metadata XLIFF source file includes all your store’s translatable metadata.The file consists of trans-unit elements that represent each unit of translatable metadata for your store. Within each trans-unit element, a `<source>` tag identifies the metadata in the store's default language. Your translator adds a `<target>` tag with the corresponding translation and includes any HTML encoding or CDATA sections that are in the source tag. Don’t modify the metadata translation source file `<source>` tags. Doing so introduces errors in the metadata.

Sample Metadata Trans-Unit (English to German)

```
<trans-unit id="Flow.Flow.RMA_Return.1.Product_Selection.Field.ProductSelectionHeading.Description" 
    maxwidth="65535" size-unit="char">
       <source><p class=&quot;ql-indent-1&quot; 
       style=&quot;text-align: center;&quot;&gt;<span 
       style=&quot;background-color: rgb(255, 255, 255); font-size: 18px; 
       color: rgb(62, 62, 60);&quot;&gt;Select from these 
       available items to return.&lt;/span&gt;&lt;/p&gt;
       </source>
       <target><p class=&quot;ql-indent-1&quot; 
       style=&quot;text-align: center;&quot;&gt;&lt;span 
       style=&quot;background-color: rgb(255, 255, 255); font-size: 18px; 
       color: rgb(62, 62, 60);&quot;&gt;Wählen Sie aus diesen 
       verfügbaren Artikeln die zurückzugebende aus.&lt;/span&gt;&lt;/p&gt;
       </target>
   </trans-unit>
   
```

#### See Also

-   [Export Metadata Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export.htm&language=en_US&type=5)
-   [Import Translated Files](https://help.salesforce.com/s/articleView?id=platform.workbench_import.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo