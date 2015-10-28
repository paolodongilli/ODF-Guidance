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

# Collaborate on documents
An overview of the different options for collaborating on ODF documents.

## Applications that support collaboration
Document solutions that implement Open Document Format (ODF) can allow different people to work together on the same document. These collaboration features can appear in:

- on-site office document applications such as those found in productivity suites (eg LibreOffice)
- open source embeddable software components
- applications run from a server (held either on-site or in the Cloud) and accessed with a web browser or desktop application

How your users share and collaborate will help determine which of these is best for your organisation.

Desktop productivity suites are probably the most familiar of these to users, but they won't necessarily be the best match for their needs. They're often complex and contain features that can be confusing, while their flexibility and portability across platforms is limited.

One of the many open source and commercially embeddable software components or out-of-the-box solutions should be able to offer users the tools they need to work effectively. You're likely to find the right one for your users' needs, whether they need to:

- use a template to compose a document that team members can easily review
- create or manage text documents contributed to by different authors
- exchange information directly with your enterprise resource planning (ERP) system or customer relationship management (CRM) database

### Web applications for collaboration
If you need to collaborate with other people on shorter text documents, a solution based on web technology is worth considering. Web applications are more:

- flexible - you can use them with people inside and outside the organisation
- convenient - every modern networked device has a browser so you don't need any installation or additional training
- cost-effective - you don't need to pay for more applications

A web browser can be used directly for document collaboration, but there are also specialised web-based collaboration tools. If you're writing longer generic text with multiple authors, such as a book or brochure, consider using a web-based writers' platform such as [BookType](https://www.sourcefabric.org/en/booktype/). It uses open source software web technology that allows authors, editors and other stakeholders to work and communicate simultaneously through the browser. The result can be exported to ODF, HTML and PDF, as well as various electronic book formats such as [EPUB](http://idpf.org/epub).

For collaboration involving a larger number of participants, an open source web commenting tool such as [Co-ment](http://www.co-ment.com/) can gather input efficiently and transparently, in a way that office applications can't.

## Collaborate offline
Offline review allows users to make comments or edits on a document regardless of whether they have a web connection, and then later share the document with other collaborators. ODF standard offers 2 basic offline review options:

- adding annotations (remarks or notes)
- using change tracking

Both annotations and change tracking can be removed automatically by web publishing software. You shouldn't add remarks inside the body of the text, as they might be left in the text and published.

### Annotations
Annotations are textual notes attached to the content of a document. They're a reliable and stable way to collaborate and work consistently across almost all applications. The content of annotations is also available through assistive technology, such as a Text-To-Speech reader.

Open source tools like [Docear](http://www.docear.org/) and [I, Librarian](https://i-librarian.net/) can sort documents and annotations into categories and let you view multiple annotations of multiple documents, in multiple categories, all at once.

### Change tracking
Change tracking lets you suggest wording within a text that the document's author may then accept or reject. Change tracking has benefits, but there are also risks you should be aware of. Not all applications implement it as a feature. See the separate chapter on change tracking (section 13 - Change tracking in ODF).

### Pre-publication tools
Documents that have been reviewed offline carry more information than you may realise. If you publish documents on your website, you might want to remove change tracking and annotations using an open source software library such as [lpOD](http://opendocument.xml.org/news/lpod-project-release-08-is-online).

Or you could use an ODF-aware commercial application like:

- [MetaClean](http://www.adarsus.com/en/metaclean.html)
- [Metadata Assistant](http://www.thepaynegroup.com/products/metadata/)
- [Datadistiller](http://www.digitalconfidence.com/DataDistiller-Metadata-Removal-Engine.html)

Some of these vendors also provide tools to actively scan and remove the change tracking information and annotations, for example in outgoing email.

## Collaborate in real time
You might want multiple people to be able to edit a document at the same time, as this can save time and be more efficient. This is often called 'collaborative real-time editing'.

Real-time collaboration solutions avoid many of the issues that users experience with offline reviewing. They offer an easy way to share, and some allow access to documents to be controlled.

Applications that allow real-time collaboration can be set up in different ways:

- peer-to-peer (directly between users)
- server-based, hosted locally within your organisation
- service-based, hosted by a third party

### Peer-to-peer (p2p)
Some ODF applications can set up collaboration directly between the devices of end users, using the same software. This is done using instant messaging or over a direct IP link. Combined with strong end-to-end cryptography p2p offers privacy and confidentiality for multi-person collaboration - only the authors and reviewers will have access to the document.

Collaborative ODF-compliant editors capable of p2p include:

- [WebODF](http://www.webodf.org/) (p2p version not yet released)
- [AbiWord](http://www.abiword.org/)
- [LibreOffice](http://www.libreoffice.org/) (p2p version not yet released)

### Server-based with local hosting
Some ODF applications can be hosted locally - ie within an organisation and connected through a local network. These include:

- web applications such as:
   - OX Apps
   - OwnCloud
   - EtherCalc
   - Bread
   - kotype
- desktop clients such as:
   - AbiWord
   - (experimental) LibreOffice

The web applications are a particularly convenient solution for both internal and external use. They don't need to be installed or updated on any device and can be used with a wide range of client devices.

### Service-based, hosted by a third party
There are some well-known ODF-aware solutions available 'as-a-remote-service' only, such as:

- [Google Docs](https://www.google.co.uk/docs/about/)
- [Microsoft Office Web apps](https://office.live.com/start/default.aspx)
- [Zoho Office](https://www.zoho.com/)

All of the applications that can be hosted within the organisation are also available as a (supported) hosted application, or can be used with any typical cloud provider.

If you use third party web tools hosted outside your organisation, you need to consider security and privacy, both for the organisation and for external users. In most cases every keystroke of every participant is sent outside of your organisation, and may well be logged elsewhere.

## Bespoke solutions
If none of the available solutions for collaboration fulfill your needs, you could:

- build on their capabilities by adding additional features
- engineer a tailored solution

Which option is most suitable for your situation depends on the needs of your users and the volume of their work.

A tailored solution might, for instance, combine document creation and editing tasks with web applications already in use in your organisation.

If you commission a bespoke solution, make sure you get the work with an open source licence to avoid future lock-in.

Try to use generic, existing open source components wherever possible, and contribute custom developed features back to the projects you've sourced them from.

For example, the open source WebODF adds ODF viewing and editing capabilities to:

- webmail clients
- content management systems (CMS) and cloud storage
- records editing in Computer Assisted Qualitative Data Analysis Software

You'll be contributing back to so-called 'upstream' open source projects, which makes the work your organisation funds reusable for others. You'll also help keep the development of these components synchronised with the software you develop.

The chapter on support and training (section 17 - Support and training) includes useful related guidance.

