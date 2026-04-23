---
title: "Language Selector"
source: "https://help.salesforce.com/s/articleView?id=experience.rss_language_picker.htm&language=en_US&type=5"
scraped: "2026-04-23"
producttype: "experience"
filter: "translat|wbench|language|locale|i18n|multilingual|localization"
---# Language Selector

Language Selector[](https://help.salesforce.com/s?language=en_US)

You are here:

1.  [Salesforce Help](/s/?language=en_US)
2.  [Docs](/s/products?language=en_US)
3.  [Experience Cloud](https://help.salesforce.com/s/articleView?id=experience.networks_overview.htm&language=en_US&type=5)

# Language Selector

Add the Language Selector component to multilingual sites so guest users can select their preferred language on public site pages.

Only guest users on public pages see the Language Selector component. The site initially appears in the default site language until the user selects a different language. The page then reloads in the selected language if a translation is available.

For authenticated users on private pages, the site typically appears in their profile language automatically. But when users have credentials and they’re not yet logged in, they’re treated like a guest user. So if a user selects a language on a public page that contains a Language Selector component—let’s say the Home page—that language choice persists after the user logs in. There are two exceptions to this rule.

-   The Login page is a public page, but even if it contains the Language Selector component, the language selection that a user makes on this page doesn’t persist after login.
-   If a user’s profile language differs from the default site language, and the user chooses the default site language in the language selector, that choice doesn't persist after login. Instead, the site appears in the user’s profile language.

To change the profile language preference as an authenticated user, open the Experience Workspace for the site that you want to view, and follow these steps.

1.  From the User Profile, click **My Settings**.
2.  From the My Personal Information menu, click **Language & Time Zone**, and select a profile language. Then when you access a site as a logged-in user, the site URL displays your selected language.
3.  To view the updated profile language, log out, and then log back in to your site.

The Language Selector component isn’t included on any page by default. Add it manually to the pages in your site. You can add the Language Selector component to any section of any page, but we recommend placing it where it’s easy to spot. Also, consider adding the component to a theme region, such as the Template Header Top region. Items that are added to theme regions are common across all pages, so it’s not necessary to add the component to every page.

Customized components and Salesforce Knowledge articles use the translations that the site admin adds through Translation Workbench.

1.  To add the Language Selector component to your page, drag it onto the page that you’re configuring.
2.  In the property editor, configure the properties for the component:
    
    | Property | Details |
    | --- | --- |
    | Label | Identifies this component on a page. This text helps increase accessibility. Default text is Preferred Language. |
    | Button Label Alignment | Specifies how the language selector’s label is aligned on the button. Select Left, Center, or Right. The default value is Center. |
    
    Note
    
    -   For information about setting up languages in a site, see [Multilingual Communities Overview](https://help.salesforce.com/s/articleView?id=sf.community_builder_multilingual_overview.htm&language=en_US&type=5). If no languages apart from the default language are set in the site, the language selector shows the default language without a dropdown option.
    -   To see the list of languages that guest users see, make sure that you’re on a page that contains the Language Selector component. Then click the selector’s dropdown icon.
    -   When a guest user accesses a site in a language that’s not included in the Language Selector component, the site redirects to the set default language in Experience Builder.
    -   A user can add the query parameters for one of the site's supported languages to the site's URL in the browser address bar and override the default site language. However, this method isn’t supported and can cause inconsistent behavior. When authenticated users want to view a multilingual site in another language, their best option is to view the site as a guest user. Or, these users can change their profile language.
    -   Ensure that all translated content and Salesforce Knowledge articles have a version in the site’s default language.
    -   Before Summer ’18, the Language Selector component was named Language Picker.
    

Example Sample Language Selector component with dropdown language list visible:

#### See Also

-   [Which Components Can I Use with Each Aura Template?](https://help.salesforce.com/s/articleView?id=experience.rss_component_reference_table.htm&language=en_US&type=5 "Aura site templates, such as Customer Service and Partner Central, are each composed of pages, which in turn are made up of customizable components. Consult this table to find out which Aura template each component can be used in, and when the component became available.")
-   [Best Practices and Considerations for Multilingual Sites](https://help.salesforce.com/s/articleView?id=experience.community_builder_multilingual_best_practices.htm&language=en_US&type=5 "Keep these practices and considerations in mind when you’re setting up a multilingual site.")

Did this article solve your issue?

Let us know so we can improve!

YesNo