---
title: "Structure of the Store Data Translation Source File"
source: "https://help.salesforce.com/s/articleView?id=commerce.comm_structure_of_store_data_translation_source_file.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "commerce"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Structure of the Store Data Translation Source File

Structure of the Store Data Translation Source File[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [B2B Commerce](https://help.salesforce.com/s/articleView?id=commerce.comm_intro.htm&language=en_US&type=5)

# Structure of the Store Data Translation Source File

The XLIFF source files for products, categories, and promotions include each object’s translatable fields. Each data source file’s element structure is specific to your store’s products, categories, or promotions. To avoid missed translations, download the XLIFF source files after your products, categories, and promotions are set for your store launch.

### Required Editions

<table class="slds-table slds-table_bordered slds-m-bottom_small edition" lwc-3eigj2skqo3=""><colgroup lwc-3eigj2skqo3=""><col lwc-3eigj2skqo3=""></colgroup><tbody lwc-3eigj2skqo3=""><tr class="" lwc-3eigj2skqo3=""><td style="vertical-align:top;" class="slds-cell-wrap" lwc-3eigj2skqo3=""><a target="_blank" href="https://help.salesforce.com/s/articleView?id=commerce.comm_editions.htm&amp;language=en_US&amp;type=5" lwc-3eigj2skqo3="">View supported editions</a>.</td></tr></tbody></table>

[Which Salesforce Commerce Product Do I Have?](https://help.salesforce.com/s/articleView?id=commerce.comm_what_product.htm&language=en_US&type=5)

The source file represents each translatable field with a trans-unit element. Within each trans-unit element, a `<source>` tag represents the corresponding field text in the store's default language. Your translator adds a `<target>` tag with the corresponding translation. If the `<source>` tag includes HTML encoding or CDATA sections, the translator includes these in the`<target>` tag.

File Modification (section tag)

You can modify a data translation source file `<source>` tag before adding the target tag translation. However, to avoid unintended errors, Salesforce recommends that you keep source tag changes to a minimum and follow these guidelines.

-   Consistency: If you modify the content within the `<source>` tags, make sure that the changes are consistent across all related files and systems. Inconsistent source text can lead to confusion and errors in translation.
-   Impact on Translations: Changing the source text will likely require retranslation of the affected content. Make sure that translators are aware of the changes and that the translations are updated accordingly.
-   Version Control: To keep track of changes to the source text, use version control. Version control helps you manage updates and understand the history of changes.
-   Context and Notes: Provide clear context and notes for any changes made to the source text. Contextual notes help translators understand the reason for the changes so they can translate accurately.

## Translatable Data Fields

You can translate product and category names and descriptions. You can also translate promotion names, promotion display names, and the terms and conditions for promotions.

Important A translated value for the data in the record’s Name field is required to translate data in other fields for that record. For example, you must provide a German translation for the name of a Product before you can translate its description into German.

Sample Product Description Translation Unit (English to German)

```
<trans-unit id=Product2.01tLT000005slQrYAI.Description maxwidth=4000 
    fieldType=MultiLineText size-unit=char>
       <source>Hi-Protein Cranberry flavored GoBars are an athletes 
       favorite with unique taste and healthy composition.</source>
       <target>Hi-Protein Cranberry-Geschmack GoBars sind ein Favorit 
    unter Sportlern mit ihrem einzigartigen Geschmack und ihrer gesunden Zusammensetzung.</target>
   </trans-unit>
```

Sample Product Name Translation Unit

```
<trans-unit id=Product2.01tLT000005slQrYAI.Name maxwidth=255 fieldType=Text size-unit=char>
       <source>GoBar Cranberry Hi Protein, 2oz - 6 pack</source>
       <target>GoBar Cranberry Hi Protein, 2oz - 6er Pack</target>
   </trans-unit>
```

Sample Promotion Terms and Conditions Transation Unit

```
<trans-unit id=Promotion.0c8LT000000C38bYAC.TermsAndConditions maxwidth=4000 
    fieldType=HtmlStringPlusClob size-unit=char>
       <source>Buy total $100 of any product from category 'Energy Bars', get 10% off entire 
       transaction from July through September 2025.</source>
       <target>Kaufen Sie insgesamt Produkte im Wert von 100 $ aus der Kategorie 'Energieriegel' und 
       erhalten Sie 10 % Rabatt auf die gesamte Transaktion von Juli bis September 2025.</target>
   </trans-unit>
```

Sample Promotion DisplayName Translation Unit

```
<trans-unit id=Promotion.0c8LT000000C38bYAC.DisplayName maxwidth=255 fieldType=Text size-unit=char>
       <source>10% Off Transaction</source>
       <target>10 % Rabatt auf Transaktion</target>
   </trans-unit>
```

Sample Promotion Name Translation Unit

```
<trans-unit id=Promotion.0c8LT000000C38bYAC.Name maxwidth=255 fieldType=Text size-unit=char>
       <source>Buy $100 of category 'Energy Bars' get 10% off transaction</source>
       <target>Kaufen Sie Produkte im Wert von 100 $ aus der Kategorie 'Energieriegel' und erhalten Sie 10 % Rabatt 
       auf die Transaktion</target>
   </trans-unit>
```

Sample Category Description Translation Unit

```
<trans-unit id=ProductCategory.0ZGLT000000Fr414AC.Description maxwidth=255 fieldType=MultiLineText size-unit=char>
       <source>Browse our large assortment of healthy energy bars.</source>
       <target>Durchsuchen Sie unser großes Sortiment an gesunden Energieriegeln.</target>
   </trans-unit>
```

Sample Category Name Translation Unit

```
<trans-unit id=ProductCategory.0ZGLT000000Fr414AC.Name maxwidth=200 fieldType=Text size-unit=char>
       <source>Energy Bars</source>
       <target>Energieriegel</target>
   </trans-unit>
   
```

#### See Also

-   [Export Metadata Translation Files](https://help.salesforce.com/s/articleView?id=platform.workbench_export.htm&language=en_US&type=5)
-   [Import Translated Files](https://help.salesforce.com/s/articleView?id=platform.workbench_import.htm&language=en_US&type=5)

Did this article solve your issue?

Let us know so we can improve!

YesNo