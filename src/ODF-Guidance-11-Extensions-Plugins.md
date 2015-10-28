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

# Extensions, plugins and custom solutions
How to ensure that software offering added functionality to document solutions meets the ODF standard.

## Additional software options
If your office productivity tools don't offer all the functions you need, additional software - extensions, plugins or add-ons (depending on the application you're using) - can help.

If you're using one of these to help create or manipulate content you should be aware of any impact this has on the output document's conformity to the Open Document Format (ODF) standard.

If you're responsible for developing an extension, plugin or add-on, consider using one of the [existing libraries that work with ODF](http://opendocumentformat.org/developers/).

## Conforming documents
ODF 1.2 compliant documents don't all conform to the standard equally. There are 2 classes for conformance:

- conforming documents
- extended conforming documents

You should produce conforming documents where possible. Using extended conforming documents may cause interoperability problems and adds complexity to documents. For instance you have to make sure that your applications can flag the document and add information to the document metadata to point to relevant information.

In most cases, extensions, plugins and add-ons to office applications can insert external data in a manner that allows a document to conform to the standard without resorting to extended conformance.

## Image or graphic plugins
Plugins that insert visual information should always use the universal mechanism for claiming a [draw area within the document]() to embed multiple alternative renderings of objects. This ensures that the content can be viewed by any conformant application and provides an editable document that's portable across applications.

You should provide:

- a vector version (using the web standard SVG) for sharp images
- a bitmap version (using the web standard PNG) as baseline
- your custom file format (encoded as base64)

Ensure that content is accessible by adding proper accessibility information (eg a title and summary description) to new objects. If the plugin has a user interface, make sure that is accessible as well.

If you use a commercial plugin, ask your vendor to ensure it's accessible. If you'd like to use an open source plugin and it lacks full accessibility features, contribute any that you develop back to the project - or commission the developers to add this relatively simple functionality.

## Validate output
If you use an add-on, plugin or extension to create or manipulate content, be aware of any impact it might have on the conformance of your document output. Use an ODF validator (see section 5 - Validators and compliance testing) to check the output.

