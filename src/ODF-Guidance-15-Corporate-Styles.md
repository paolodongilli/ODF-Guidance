<!--
Copyright (C) 2015 Crown Copyright
Copyright (C) 2015 Paolo Dongilli

List of contributors:
- Cabinet Office, UK Government
- Paolo Dongilli, Autonomous Province of Bozen-Bolzano, South Tyrol, Italy
- ADD YOUR NAME HERE

This file is part of the document "Open Document Format (ODF) - A Guidance for Governments" which is licensed under the terms of the Open Government License v3.0 (http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

The whole document is a revised version of the document "Open Document Format (ODF): guidance for UK government" released by the Cabinet Office of the UK Government as of 11 September 2015. The original document can be found at https://www.gov.uk/guidance/open-document-format-odf-guidance-for-uk-government, licensed under the same Open Government Licence v3.0.
-->

# Corporate styles and templates
Best practice for working with styles and templates in ODF.

##Styles and templates
Open Document Format (ODF) offers advanced style and template functions across office document applications. You should be aware of general good practice and specific considerations for working with and managing styles and templates in ODF.

### Styles
A style is a bundle of formatting properties that can be applied to a specific document element or any part of it. It can specify typeface, font size and characteristics such as:

- where elements are placed and what the context should look like, including margins, padding, borders, backgrounds
- page breaks before and after an instance of a certain style
- specific language for the element involved
- whether a certain type of numbering needs to be applied
- automatically generating a table of contents from the headings in the document

Creating and applying styles to documents instead of directly formatting them enables you to:

- maintain a consistent corporate identity in documents
- maintain a document's structure
- create documents that are accessible to people using assistive technology
- automate the process of converting documents to other types of content eg DAISY audio content
- help people focus on creating good content rather than managing style and formatting

### Templates
Templates are blank documents pre-configured with text and style elements that are relevant and common to particular document needs. Your organisation will have a set of styles used across templates and documents.

### Styles and templates in ODF
ODF applications typically come with a set of predefined styles, such as 'Heading 1', 'Title' or 'Footnote'.

A paragraph style can be set to automatically have another style follow it. 'Heading 1', for instance, is usually followed by a style called 'Content Body', 'Default' or 'Normal'. Companies can add their own styles to a template.

The OASIS specification of the ODF file format has text styles similar to 'variable name' and 'variable default value', which allow values to be automatically extracted from the document.

ODF template documents have the following file extensions:

- .ott (texts)
- .ots (spreadsheets)
- .otp (presentations)
- .otf (formulas)
- .otg (graphics)
- .otc (charts)
- .oti (images)
- .oth (HTML output)

## Create templates and styles
When creating templates and styles:

- begin with a blank template and keep interoperability in mind
- prefer features that are mandatory for conformant applications over optional features in the standard
- avoid constructs that don't add much value, such as frames in frames
- include proper fallbacks for images.
- ensure templates are suitable for users of assistive technology
- use a validator to make sure template documents fully conform to the ODF specification
- test templates and documents in the important applications people inside and outside your organisation - work with (the [Officeshots.org](http://officeshots.org/) tool can be used for this)
- embed any fonts used that might not be available on every platform
- train users how to work with templates and styles

## Keep templates up to date
Organisations typically use many templates, most of which will be derived from a smaller set of root templates. When these root templates need to change all the templates that were derived from them will also need to be changed.

You may need to update installed templates to allow for:

- new features
- design changes
- interoperability issues

When multiple versions of the same template exist it can be unclear which documents use which version. Adopting a proper naming and versioning scheme for your templates can help avoid this confusion. This can, for instance, allow your organisation to later re-apply a new version of a template automatically when the corporate style is updated.

When you've used a template to create a new document, an application can [link to the template](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-part1.html#__RefHeading__1415114_253892949) (or a specific version of that template) inside the document metadata. You may also want to [insert the name of the template](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-part1.html#__RefHeading__1415320_253892949) in the visible text of a document (eg in a footer) to help identify the template used where it might not be otherwise obvious (ie in a print flow based on a number of different templates that sometimes vary).

Organisations using many templates in a complex hierarchy should consider managing them with a dedicated standalone tool. An online ODF template generator such as [DocGen](https://joinup.ec.europa.eu/software/docgen/description), for example, can allow different departments to create custom ODF templates using a pre-approved set of variants. Log custom templates so updates can be made to the root templates they were based on. New custom templates can then be automatically generated and distributed. This solution directly interfaces with office applications but can also be integrated with document lifecycle management tools and mid-office applications. Browser-based tools are also available.

## Dynamic content in templates
ODF applications let you insert dynamic content in a template using

- variables (the most common option and a fairly reliable one)
- form functionality
- preprocessor or plugin

Embedded macros aren't good practice.

### Variables
You can create templates to automatically insert or hide specific information depending on the context. Contextual variables might include:

- a page number
- the number of pages in a document
- the current date
- user-defined variables from the document's metadata or other source the application is aware of

Variables can be displayed in a document using so-called variable fields, but can also be used as conditionals (ie if/then determinants).

### Form functionality
Sometimes a template requires input from users to generate documents. ODF includes a form functionality that permits this. Based on a standard called [XForms](http://www.w3.org/TR/xforms/), form support in ODF allows high levels of interaction, is flexible and safe, and can be charged on a per template basis.

Your organisation could also consider:

- using a web application (browser-based tools are better than document formats for collecting information)
- building a custom application with an office library like [Calligra](http://calligra.org/) or [Aspose](http://aspose.com/), to provide a streamlined user experience that avoids the use of an office application altogether
- integrating with the office application using a plugin or extension

