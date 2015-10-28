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

# Integrate ODF with enterprise tools
How ODF fits into the way your organisation processes documents.

## Enterprise tools
Enterprise tools are software applications that perform specific processes that an organisation needs, rather than its individual users, such as record and document management. Office documents will often be processed in some way by enterprise tools, which can involve:

- pre-processing (eg creating a template letter using information from a case management system)
- post-processing (adding an electronic signature or annotating the document)
- other kinds of manipulation or modification

Enterprise tools are often embedded in an organisation's working practice. They'll need to be carefully integrated with your document solutions to ensure they work with Open Document Format (ODF).

## Choose a platform
You'll need to decide what platform you'll use to integrate enterprise tools with ODF. Your choice should depend on your users' needs.

Web-based solutions have advantages over office applications. They

- don't require installation or updates on your user devices
- are less complex
- are available for use on devices other than just desktops
- are less prone to user error

If you need convenient access to rich text editing, making charts or adding corporate branding then web-based solutions might not be appropriate. Office applications can offer these, but there are also dedicated software components that allow you to integrate office viewing and editing capabilities into your own software. For example:

- libraries such as the open source [Calligra](https://www.calligra.org/) Engine or [Aspose](http://www.aspose.com/) natively work with ODF and allow easy integration
- into desktop, server and server-side web applications
- the open source [WebODF](http://www.webodf.org/) framework is built around ODF viewing and editing within client-side web applications

## Automate tasks and processes
If you're using office applications in combination with macros to assemble documents and carry out tasks, you can probably do the same thing more easily and cheaply with ODF. You should move avoid using macros when possible to avoid issues with security and interoperability. ODF allows you to assemble documents and automate:

- different stages in a process
- repetitive tasks
- reports or presentations from business data

Many software libraries can process documents from different sources, allowing you to assemble and manipulate the content in different ways. Most are easy to use, offer advanced functions and require little knowledge of ODF.

## Records and documents management
Keep structured information intact and accessible in an automated way, close to the original source of the data. There should be one authoritative source where all information that belongs together is maintained.

For instance, if you have a collection of documents that have been created by mail-merge from a database, you should save the database as your record, not the individual letters in their document format. Using one or more office applications to maintain separate, stand-alone documents makes it much more difficult to manage that information or get a clear overview of it.

## Use metadata to record a document's history
Once your content has been moved into ODF, you should keep information well-structured and complete. For quality assurance you need to trace where your information is modified, by whom or what, and how. You can do this by using metadata, which is data about other data - in this case describing the information in your document. Metadata features in ODF allow you to keep track of what happens inside your documents, from the moment they're generated until they're archived.

When attaching metadata you should:

- specify which document template was used to create a series of documents, so you can make updates easily when the template is replaced
- make it clear what part of a document is modified by automated software and what version of the software you're using by setting the meta:generator tag or other relevant meta-tags
- enable version control (change tracking) by default where a person will modify a document generated by an application; you can see the history of the document, scan for errors and other integrity issues and trace the impact of mistakes throughout the entire application chain
- add a digital signature to a document if the integrity of information contained in it is important
- place scripting or placeholder instructions in a logical place, preferably inside user variables or script tags

## Create new ODF templates
When creating new ODF templates make sure that:

- they are clean and technically sound
- they have been verified to work in the most common applications
- fonts and sizes are included in the template

Add the appropriate accessibility information for anyone who will be working with your document, including people who need assistive technology.

If you have to convert legacy templates you should:

- validate every step in the process
- make sure the manifest is complete
- make sure all reference styles are defined

See the section about validators and compliance testing (section 5 - Validators and compliance testing).

## Replace legacy applications incompatible with ODF
You should consider replacing legacy applications that can't work with ODF. Most of the tools needed to work with ODF are low-cost (or free) compared to traditional solutions and office applications. As an interim step, create documents using XML, JSON or structured text output using one of the tools available in the software library.

If no compatible outputs are available from your product, you may need to work with the best possible option your vendor provides and then create the output in ODF as you need it. Many office applications offer a non-interactive batch mode that can be used for conversions. Alternatively there are external tools like OfficeConvert for Microsoft Office, which was produced for the ODF validation service [Officeshots](http://officeshots.org/).

Converting documents from legacy formats can be inefficient but manageable unless your output is unpredictable. Validate your output and clean up the results to prevent processing errors in future.

## Don't use direct formatting
Never manually change the font type, font colour, background or letter spacing in template or document generation software. You should always use styles and headings, otherwise there will be information loss for people using assistive technology, search engines and PDF generators, among other tools.

## Variable data printing
Variable data printing involves printing very large numbers of documents (ie hundreds of thousands or even millions) generated from, for example, large mail merges. If your organisation does variable data printing, the content of your ODF compatible office documents will need to be converted to [PPML](http://www.standards.podi.org/ppml/ppml-overview.html) (Personalised Print Markup Language). PPML is a dedicated standard for high performance printing of large volumes of nearly identical documents. Like ODF it's an XML language, which allows standard XML technologies such as XSLT to automatically convert parts of documents created in ODF to PPML-ready assets.

