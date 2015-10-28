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

# Change tracking in ODF
An overview of the change tracking options in ODF: their benefits, risks and alternatives.

## Options that support change tracking
Change tracking lets reviewers suggest new wording, which the document's author may accept or reject. It's an optional feature of the Open Document Format (ODF) standard, which is supported by many open source editors including:

- [Apache OpenOffice](https://www.openoffice.org/)
- [EuroOffice](http://www.multiracio.com/index.php?style=eurooffice&page=eo)
- [LibreOffice](https://www.libreoffice.org/)
- [NeoOffice](https://www.neooffice.org/neojava/en/index.php)

It's a relatively complex feature to implement.

Only some current versions of Microsoft Office can record change-tracking information when saving a document to ODF. If a user adds tracked changes in an unsupported format, these may be accepted automatically and not tracked when the document is converted to ODF.

Older versions of Microsoft Office that used the open source ODF Converter Add-in did have change tracking capabilities, so if your users are on an older version of Microsoft Office and need the feature, the source code of the add-on is available.

## Risks and benefits
Change tracking has both benefits and potential risks.

The benefits are that:

- a reviewer's suggested changes can be approved or rejected quickly
- an editor can easily switch between displaying the text with proposed revisions made and the original text with the changes suggested

The risks are that:

- change tracking might be applied inconsistently, as users can easily forget to turn on change tracking, or may have turned it off and on again
- changes might not all be correctly captured, especially if people are using different applications, old versions of software or mobile apps
- a document might be infected by a virus or other malware
- the change tracking log might be incomplete: other, unlogged changes might have been made

## Automatically compare documents
There are also ways to compare different versions of ODF documents so you can see what changes were made. The different options for this include:

- through a feature available in some office applications
- standalone applications or services, such as tools that highlight all the differences between 2 versions of a document for manual inspection (eg [DeltaXML ODT Compare](http://www.deltaxml.com/products/odt_compare/))
- other standalone solutions (eg a plugin that can be integrated into an office suite)

## Automated multiway merging
If your organisation sends longer documents to many reviewers, manually comparing them may not be efficient because the editor will receive too many modified copies containing changes or textual suggestions.

Automatic merging software can be a solution in this case by allowing you to:

- accept or reject changes from multiple reviewers while working on just one document
- group small adjacent changes together for easier comparison
- optionally ignore markup changes when they represent disallowed formatting

Automated multiway merging can be particularly useful when you're:

- working on large documents with multiple authors and need strict control
- resolving conflicts that might occur when multiple users check in the same edited document
- rejoining independently authored versions of some original text

## Alternatives
Alternatives to change tracking include annotations, real-time collaborative editing and web-based collaboration tools. See the chapter on document collaboration (section 12 - Collaborate on documents).

