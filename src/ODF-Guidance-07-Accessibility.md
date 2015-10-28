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

# Accessibility
How to ensure your ODF document solution is accessible to people with disabilities.

## The accessibility requirement
Many people with disabilities have trouble accessing office documents without assistive technologies or inclusive design. Disabilities that can make working with documents difficult include, but aren't limited to:

- visual impairments
- motor impairments
- cognitive impairments

The severity of these disabilities can vary widely. Visual disabilities, for example, can range from colour vision deficiency (which affects roughly 8% of the male and 0.5% of the female population globally) to total blindness.

You must take appropriate steps to ensure that people with disabilities can access the content of office documents as easily as possible. This can be either through adaptive technologies, such as screenreaders or alternate input devices, or through universal, inclusive design - ie one design directly accessible to those with and without disabilities.

In the UK, to exclude a user on the basis of disability would breach the Equalities Act 2010. See the Service Design Manual for more [information on accessibility](https://www.gov.uk/service-manual/user-centred-design/accessibility).

## Make documents more accessible
There are 2 ways to make office documents more accessible:

- appropriate formatting by the author
- automated processes in the applications used to create them

The Canadian Accessible Digital Office Document (ADOD) project has produced [detailed guidance for improving office documents](http://inclusivedesign.ca/accessible-office-documents) to make them more accessible, including word-processing documents, spreadsheets, presentations and e-books. These guidelines are meant for documents that are:

- intended to be used by people (ie not computer code)
- text-based (ie not simply images, although they may contain images)
- fully printable (ie where dynamic features are limited to automatic page numbering, table of contents, etc and do not include audio, video, or embedded interactivity)
- self-contained (ie without hyperlinks to other documents, unlike web content)
- typical of office-style workflows (reports, letters, memos, budgets, presentations, etc)

There is also [guidance on creating accessible content](https://www.gov.uk/service-manual/user-centred-design/accessibility.html) in the UK Government Service Design Manual.

## Product-specific support
Some productivity tools have better support than others for the accessibility features included in the Open Document Format (ODF) specification.

Tools with high quality support include:

- Microsoft UI Automation with Microsoft Office
- the combination of IAccessible2 API with Apache OpenOffice (as of version 4.1) and LibreOffice (as of version 4.3)
- Microsoft Office Online (part of Office 365), which provides WAI-ARIA support for assistive technologies (WAI-ARIA stands for Web Accessibility Initiative-Accessible Rich Internet Applications)
- Office Online where you use an assistive technology such as a screen reader or speech recognition software, if the assistive technology supports WAI-ARIA

Previously included as part of Microsoft Office, speech recognition is now available as part of the Windows operating system. If you use Microsoft Windows XP and need speech recognition, you need to use an older version of Microsoft Office with the ODF converter plugin.

AccessODF is a useful extension for Writer (the word processing application in LibreOffice and Apache OpenOffice) that helps improve the accessibility of text documents. Recent versions of Microsoft Word include an integrated checking function.

Product-specific information on accessibility is available for:

- [Apache OpenOffice](http://accessodf.sourceforge.net/)
- [Google Apps](https://support.google.com/a/answer/1631886?hl=en)
- [LibreOffice](https://www.libreoffice.org/get-help/accessibility/)
- [Microsoft Office 2013](https://support.office.com/en-za/article/Accessibility-features-in-Office-2013-be8d4909-d025-4049-9e1c-ac608ec53edb)
- [Microsoft Office 365](https://www.microsoft.com/enable/products/office365/)

## ODF support of alternative media
ODF supports braille, large-print, and audio alternatives to print and e-documents. Audio is particularly important, as it provides access to documents for many people with disabilities such as visual impairment or blindness and learning disabilities.

When implemented correctly, these and alternative input methods will help users with disabilities to read, create, and edit documents - with full access to all of the meaning and intent. A blind person, for example, should be able to work with a document someone else created by getting a text description of the images used. A person should if needed be able to fill out a form without using hands. Someone with poor vision should be able to read presentation materials easily.

Automatic open source converters are available for easy conversion from ODF to braille, and from ODF to the DAISY audio book standard.

## Build solutions that implement accessibility
While ODF offers accessibility features, whether they're available and how well they'll function will depend on how successfully the standard is implemented in applications and assistive technologies.

Many blind users depend on third party assistive technologies, many of which are hardwired to a limited set of established products and platforms. These products should continue to support user workflow seamlessly if they support ODF 1.2 well.

If your organisation selects other products, make sure adequate assistive technologies are available as well - or allow exceptions.

It's relatively straightforward to support the main accessibility features such as text labels and object descriptions coming from an application. Find out which assistive technology requirements your users have, and talk to vendors. If you don't have the technical capabilities in your organisation to do so, pool together with others or hire experts. Build in enough time and think ahead: this will allow for the most cost-effective solutions. Vendors will often be receptive to reasonable bids for making their existing solutions more accessible. Accessibility is something both vendors and open source communities want, but often lack the budget for.

## ODF accessibility guidelines for developers
The ODF technical subcommittee on office accessibility has ensured that versions 1.1 and 1.2 (the current version) of the ODF standard support encoding to make documents accessible through assistive technologies. There are detailed [accessibility guidelines](http://docs.oasis-open.org/office/office-accessibility/v1.0/cd02/ODF_Accessibility_Guidelines-v1.0.html) for version 1.1. Written for developers, the guidelines include detailed information on approaches to accessibility for different categories of disability. They're also a useful resource for anyone interested in accessibility issues for productivity software.

