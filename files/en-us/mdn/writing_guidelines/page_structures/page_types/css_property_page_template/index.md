---
title: CSS property page template
slug: MDN/Writing_guidelines/Page_structures/Page_types/CSS_property_page_template
page-type: mdn-writing-guide
tags:
  - meta
  - writing-guide
browser-compat: css.properties.NameOfTheProperty
---

{{MDNSidebar}}

> **Note:** _Remove this note block before publishing._
>
> ---
>
> **Page front matter:**
>
> The front matter at the top of the page is used to define "page metadata".
> The values should be updated appropriately for the particular property.
>
> ```md
> ---
> title: NameOfTheProperty
> slug: Web/CSS/NameOfTheProperty
> page-type: css-property OR css-shorthand-property
> tags:
>   - CSS
>   - Reference
>   - CSS Property
>   - NameOfTheProperty
>   - Experimental
>   - Deprecated
> browser-compat: css.properties.NameOfTheProperty
> ---
> ```
>
> - **title**
>   - : The title heading is displayed at the top of the page. The title format is _NameOfTheProperty_.
>     For example, the [`background-color`](/en-US/docs/Web/CSS/background-color) property has a title of _background-color_.
> - **slug**
>   - : The `slug` value is the end of the URL path after `https://developer.mozilla.org/en-US/docs/`. This will be formatted like `Web/CSS/NameOfTheProperty`.
>     For example, the [`background-color`](/en-US/docs/Web/CSS/background-color) property slug is `Web/CSS/background-color`.
> - **page-type**
>   - : The `page-type` key for CSS properties is `css-shorthand-property` for shorthand properties; otherwise it is `css-property`. For example, the `page-type` value for the [animation](/en-US/docs/Web/CSS/animation) property is `css-shorthand-property` but for the the [animation-delay](/en-US/docs/Web/CSS/animation-delay) property, it is `css-property`.
> - **tags**
>
>   - : Always include the following tags: **CSS**, **Reference**, **CSS Property**, _NameOfTheProperty_ (e.g., **background-color**).
>
>     Include the following tags as appropriate:
>
>     - Category of property: **Layout**, **Graphics**, **CSS Background**, **CSS Colors**, or other tags as appropriate
>     - Technology status: [**Experimental**](/en-US/docs/MDN/Writing_guidelines/Experimental_deprecated_obsolete#experimental)) or [**Deprecated**](/en-US/docs/MDN/Writing_guidelines/Experimental_deprecated_obsolete#deprecated_and_obsolete))
>     - Others: Any other terms related to the technology that people might search for
>
> - **browser-compat**
>
>   - : Replace the placeholder value <code>css.properties.NameOfTheProperty</code> with the query string for the property in the [Browser compat data repo](https://github.com/mdn/browser-compat-data).
>
> ---
>
> **Top-of-the-page macros**
>
> A number of macro calls appear at the top of the content section (immediately below the page front matter).
> You should update or delete them according to the advice below:
>
> - `\{{SeeCompatTable}}` — this generates a **This is an experimental technology** banner that indicates the technology is [experimental](/en-US/docs/MDN/Writing_guidelines/Experimental_deprecated_obsolete#experimental).
>   If the technology you are documenting is not experimental, you can remove this.
>   If it is experimental, and the technology is hidden behind a pref in Firefox, you should also fill in an entry for it in the [Experimental features in Firefox](/en-US/docs/Mozilla/Firefox/Experimental_features) page.
> - `\{{Deprecated_Header}}` — this generates a **Deprecated** banner that indicates that use of the technology is [discouraged](/en-US/docs/MDN/Writing_guidelines/Experimental_deprecated_obsolete#deprecated_and_obsolete).
>   If it isn't, then you can remove the macro call.
> - `\{{CSSRef}}` — this must be present on every CSS property page. It generates a suitable CSS sidebar, depending on what tags are included on the page.
>   Remember to remove the `\{{MDNSidebar}}` macro when you copy this page.
>
> ---
>
> **Other macros in the page**
>
> - Formal definition and Formal syntax sections: The content of the _Formal definition_ and _Formal syntax_ sections is generated in place of the `\{{CSSInfo}}` and `\{{CSSSyntax}}` macros, respectively. For these sections to have data, you must ensure an appropriate entry has been filled in for the property in our [properties.json](https://github.com/mdn/data/blob/main/css/properties.json) data file. See [properties.md](https://github.com/mdn/data/blob/main/css/properties.md) for more information.
> - Specifications and Browser compatibility sections: The build tool automatically uses the `browser-compat` key-value pair to insert data into the Specifications and Browser compatibility sections (replacing the `\{{Specifications}}` and `\{{Compat}}` macros in those sections, respectively).
>
>   Note that you may first need to create/update an entry for the property and its specification in our <a href="https://github.com/mdn/browser-compat-data">Browser compat data repo</a>.
>   See our [compatibility tables guide](/en-US/docs/MDN/Writing_guidelines/Page_structures/Compatibility_tables) for information on adding or editing entries.
>
> _Remember to remove this note block before publishing._

{{SeeCompatTable}}{{deprecated_header}}{{CSSRef}}

In the introductory paragraph, start by naming the property and saying what it does.
This should ideally be one or two short sentences.

## Try it

_This title is auto-generated by the macro `\{{EmbedInteractiveExample}}`._

This section is for interactive examples added using the `\{{EmbedInteractiveExample}}` macro. See the [Interactive example demo](/en-US/docs/MDN/Writing_guidelines/Page_structures/Code_examples#interactive_example_demo) section in our writing guidelines for more information.

## Constituent properties

Add this section only for shorthand properties, such as [animation](/en-US/docs/Web/CSS/animation), to list all the related longhand properties.

## Syntax

Include the common use cases as a code block and describe the component subvalues that make up a complete value.

```css
/* Insert code block showing common use cases */
/* or categories of values */
```

### Values

Include one term and definition for each subvalue.

- subvalue1
  - : Include a description of the subvalue, its data type, and what it represents.
- subvalue2
  - : Include a description of the subvalue, its data type, and what it represents.

## Description

This is an optional section to include a description of the property and explain how it works. Use this section to explain related terms and add use cases for the property.

## Formal definition

`\{{CSSInfo}}`

_Remember to remove the backticks and backslash to use this macro._

## Formal syntax

`\{CSSSyntax}}`

_Remember to remove the backticks and backslash to use this macro._

## Examples

Note that we use the plural "Examples" even if the page only contains one example.

### Add a descriptive heading

Each example must have an H3 heading (`###`) naming the example. The heading should be descriptive of what the example is doing. For example, "A simple example" does not say anything about the example and therefore, not a good heading. The heading should be concise. For a longer description, use the paragraph after the heading.

See our guide on how to add [code examples](/en-US/docs/MDN/Writing_guidelines/Page_structures/Code_examples) for more information.

> **Note:** Sometimes you will want to link to examples given on another page.
>
> **Scenario 1:** If you have some examples on this page and some more examples on another page:
>
> Include an H3 heading (`###`) for each example on this page and then a final H3 heading (`###`) with the text "More examples", under which you can link to the examples on other pages. For example:
>
> ```md
> ## Examples
>
> ### Using the fetch API
>
> Example of Fetch
>
> ### More examples
>
> Links to more examples on other pages
> ```
>
> **Scenario 2:** If you _only_ have examples on another page and none on this page:
>
> Don't add any H3 headings; just add the links directly under the H2 heading "Examples". For example:
>
> ```md
> ## Examples
>
> For examples of this API, see [the page on fetch()](https://example.org).
> ```

## Accessibility concerns

This is an optional section. You can include any warnings here for accessibility concerns that developers should be aware of while using this property. You can also include workarounds for these accessibility concerns if there are any.

## Specifications

`\{{Specifications}}`

_Remember to remove the backticks and backslash to use this macro._

## Browser compatibility

`\{{Compat}}`

_Remember to remove the backticks and backslash to use this macro._

## See also

Include guides relating to the current property or a list of other properties here.

- link1
- link2
