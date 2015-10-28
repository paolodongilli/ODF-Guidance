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

# Introduction to Open Document Format (ODF)
An overview of ODF, how it works and why your organisation should use it.

## ODF's main properties and features
Open document format (ODF) has been an [international standard](http://www.iso.org/iso/home/standards.htm) for software since 2005. Herein we suggest all governments, as the UK government does, to use ODF for creating editable documents.
 
ODF allows users to send, view and share office documents regardless of what software they have and what device (e.g. tablet, mobile, laptop) they are using. To do this, ODF puts different types of office documents into a single file format that covers:
- text documents
- spreadsheets
- charts
- graphical documents, such as drawings and presentations

ODF also provides other useful features, such as:

- a track changes mechanism (which will be extended to offer [real-time collaborative editing](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=office-collab))
- the ability to add [digital signatures](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-part1.html#__RefHeading__1415064_253892949) to a document
- a powerful generic [metadata](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-part1.html#__RefHeading__1415064_253892949) system

ODF consists of a family of technical specifications put together by an international consortium called [OASIS](https://www.oasis-open.org/). OASIS includes representatives from hundreds of large and small software companies as well as academics, government representatives, civil society representatives and other stakeholders.

The current version is [ODF 1.2](http://docs.oasis-open.org/office/v1.2/OpenDocument-v1.2.html) and this is the version the government has adopted.

## How ODF works
Many users won't notice a difference when they use files saved in ODF. ODF keeps the document's content and layout information separate so that they can be processed independently of each other. Each type of object in the file is given its own place, and there's a neat index of every subfile inside. This unlocks powerful new capabilities for office applications that were not available in earlier file formats, such as embedded [Linked Data](http://data.gov.uk/linked-data).

ODF is not tied to a single supplier and could be used by any supplier in any product. It also provides a flexible container that can embed almost any existing digital object and allow it to be used in an office document. Custom metadata (such as [provenance data](http://www.w3.org/TR/prov-overview/), [copyright information](http://commonsmachinery.se/) and other forms of Linked Data) can be added anywhere, to any element within a document.

This is similar to how the HTML standard allows you to reference just about anything, such as:

- a TIFF image file from a 30 year old scanner
- a plugin object from a third party supplier (eg Adobe Flash)
- a custom font used to style a page

HTML does not define any of these, but just has to point to the right place.

Similarly, ODF opens many possibilities for integrating with business processes and internal applications. It allows you to, for example:

- embed a live webpage inside a presentation
- include a complete music score within a text document
- put a zoomable 3D globe inside a spreadsheet to show where your organisation is buying the most products and services

ODF is built on another common standard called [XML (Extensible Markup Language)](http://www.w3.org/standards/xml/), a well-known web standard for structured data created by the [World Wide Web Consortium (W3C)](http://w3.org/). This has helped make a versatile standard that has been quickly adopted in the marketplace. ODF specifications reuse quite a few other W3C standards, such as [RDF metadata](http://www.w3.org/RDF/), [Synchronised Multimedia](http://www.w3.org/AudioVideo/) and [digital signatures](http://www.w3.org/Signature/).

## Reasons your organisation should use ODF
The ODF standard has been [adopted for use by UK government organisations](https://www.gov.uk/government/news/open-document-formats-selected-to-meet-user-needs). It's used by governments across the world and supports the functionality that most users expect in modern office productivity software.

### ODF allows you to work with a wide range of tools and devices
In the past, IT departments didn't need to take into account users outside their organisation when they were procuring office applications. Documents were created in a single office application and would travel electronically to a single brand of printers in the print room. External users weren't affected by the choices IT departments made.

Now most organisations have to interact with many external users on a daily basis. Because of that, IT departments have to start with user needs (see section 4 - Base ODF solutions on user needs) when they tender a contract for a new supplier.

Users can now create, collaborate and interact on a wide variety of devices, platforms, software tools and services. They should also be able to access government information without having to buy expensive software. ODF's goal is to make information accessible to all, regardless of the device they are using or the software they have.

Some people and businesses may have a specific need for customised software and hardware. You can't give a sight impaired employee a tablet app to do their work at the service desk of a supplier. Likewise, a private law firm will have different needs and financial means compared to a charity or local court.

Users need software and technology to work together seamlessly, because the output from one organisation is the input of the next. ODF helps provide the interoperability that will allow everyone to choose the tool that best meets their needs.

### ODF is flexible, versatile and lowers IT costs
ODF shares many of the traits that are common between web- and device-based applications. For example, many office applications offer access to online editing environments through a web browser. This shared technology:

- lowers the cost for implementing ODF
- creates an economy of scale
- increases the product's robustness
This shared technology allows users to benefit from the availability of [Linked Data](http://data.gov.uk/linked-data) and to become part of it. Combining ODF with other XML data means that the structured information inside can be reused or consumed in ODF.

As ODF isn't tied to a single supplier, different suppliers can offer additional solutions that should be compatible with your existing ODF applications. The potential for healthy competition can help keep costs down.

### ODF allows you to store and access information over the long term
Many older office files are made up of long binary sequences. Numbers, words, formatting and other information you enter as you type and click are converted into long rows of zeroes and ones. These make no sense outside of the specific applications that created them, so that application is needed to read that information. Interpreting a single bit of this binary code incorrectly could cause the application reading that file to behave in the wrong way. And there's no easy way to tell if errors occurred.

Understanding files written in these legacy formats is challenging even for experts, including the software developers that have written applications that process them. Some file formats also have reached the end of their lifecycle and are no longer maintained by their original creator, for instance the various versions of .doc, .xls, .ppt and .wpd. ODF is the universal, supplier-neutral successor to all of these legacy formats.

Beyond the user needs of today, governments also have to consider future needs. Users need to be able to access many types of documents in the long term, including records, birth certificates and legal documents such as permits about property ownership or contracts.

ODF is an advanced and future-proof format that can cater for these needs.

### ODF keeps your organisation's data more secure
Using ODF can help make organisations much less vulnerable to targeted attacks compared to older binary (legacy) formats. This reduces the number of computers infected by viruses, spyware and adware. Legacy office files are among organisations' top 3 most common vulnerabilities to targeted attacks.

[German research in 2011](http://www.odfplugfest.de/sites/default/files/20110715_odfplugfest_caspers_zendel.pdf) indicated that the effectiveness of antivirus applications tested against attacks carried out through legacy text document files was limited. Three out of 4 antivirus solutions scored a recognition of 20% or less.

Legacy file formats (such as .doc, .xls and .wpd) were created when resilience against cyber attacks wasn't a significant part of design requirements, as computers were typically offline. The proprietary nature of these formats means you can't run a machine processable set of validation rules (see section 5 - Validatiors and compliance testing) to check if a document contains something unusual.

Binary documents make it easy to hide active attack software as the software used in an attack will often consist of short streams of zeroes and ones.

Of course, ODF itself does not make insecure software safe. It can only make it easier to check exactly what is going in and coming out of the document. It is up to the individual application and anti-malware measures to protect you and the people you communicate with.

## Who maintains and develops ODF
The [Open Document Format for Office Applications Technical Committee (ODF TC)](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=office) produces and maintains ODF.

Current [members of the ODF TC](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=office) include:

- publicly traded companies (such as IBM, Microsoft, Red Hat and Beijing Venustech), small and medium enterprises
- a number of open source communities (Multiracio, Collabora Productivity Ltd, The Document Foundation, KDE e.V.)
- independent industry experts and representatives of [ISO/IEC JTC1 SC34](http://www.jtc1sc34.org/)

SC34 is a sub-committee of the [International Standardization Organization (ISO)](http://www.iso.org/) and [International Electrotechnical Commission (IEC)](http://iec.ch/) committee.

OASIS is officially responsible for maintaining the ODF standard, but ODF is also officially published as an [International Standard ISO/IEC 26300](http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=43485) by ISO/IEC JTC 1.

Anyone can participate within OASIS directly or through membership of a national standards body such as the [BSI](http://www.bsigroup.com/en-GB/).

You can also send comments to a [public mailing list](https://lists.oasis-open.org/archives/office-comment/) maintained by the ODF TC members.

