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

# Procure ODF solutions
An overview of steps you should take when procuring applications or services dealing with editable documents, to ensure they comply with the ODF standard.

## Buy products and services based on ODF
When procuring an application, product or service that deals with editable documents and their lifecycle you must make sure your specification includes ODF compliance. Editable documents include text documents, spreadsheets and presentations. A document's lifecycle involves creation, viewing, changing (including revisions), exchanging and archiving.

> Documents that are for viewing rather than editing, e.g. PDFs, must also comply with a [separate set of open standards](https://www.gov.uk/government/publications/open-standards-for-government/viewing-government-documents). Read about open standards and how they relate to procurement in the UK government's [Open Standards Principles](https://www.gov.uk/government/publications/open-standards-principles).

Make sure the ODF requirement for services and products is clear in your tender documentation, particularly in the tender specification. Your contract should specify that the supplier is required to ensure ODF support at the time of deployment, according to the agreed specifications and requirements.

## ODF requirements for tendering
Include a clear statement in your technical specification of your functional and user needs (see section 4 - Base ODF solutions on user needs) so that suppliers can make sure that the proposed solution meets them. Review the government policy paper on sharing or collaborating with government documents (an example from the UK can be found here [https://www.gov.uk/government/publications/open-standards-for-government/sharing-or-collaborating-with-government-documents](https://www.gov.uk/government/publications/open-standards-for-government/sharing-or-collaborating-with-government-documents) to help prepare your statement. You can also download and use [this sample text](https://www.gov.uk/government/uploads/system/uploads/attachment_data/file/418651/ODF_procurement_sample_text.odt) for ODF procurement specifications.

### Core requirements
Your procurement documentation must include the requirement that the application or service works reliably with revisable ODF text documents, spreadsheets and presentations for purposes of:

- generating
- importing
- viewing
- editing
- storing
- tracking changes (where required; specify that ODF documents keep track of changes to the document so they can be reviewed and individually approved or rejected)

### Full support for ODF
You should also ensure that:

- products retain all relevant information when storing output in ODF or importing or exporting data
- there are no dependencies on other file formats
- suppliers don't hardwire their software with a specific office application but not support the standard

### Solution-specific extensions
ODF is able to incorporate 'foreign elements'. These are data elements that can be added to give software developers some flexibility to offer added functionality. These foreign elements may make documents less portable (ie possibly incompatible with some other tools) and can make functionality more difficult to migrate from one solution to another. If a different application can't interpret the meaning of some elements within a document, it won't be able to make use of the information it contains.

You should understand where and how software makes use of such [foreign elements](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-part1.html#ForeignElementsAndAttributes). You should state in the procurement documents that suppliers should provide complete documentation about any foreign elements used in their software. You may request sample documents to test in multiple applications, or ask suppliers to demonstrate compliance with an ODF validator (see section 5 - Validators and compliance testing).

You should ask suppliers to address how they use and handle foreign elements when submitting their tender.

### Cross-platform use
Any product or service you procure should allow editable documents to work equally well across platforms (ie, different software, operating systems and devices). If you create a document in ODF using the proposed solution on one platform, you should be able to read, modify and save it on another - and vice versa. Make sure the supplier gives you the necessary information to test functionality between various platforms.

## Supplier confirmation of ODF support
You should ask potential suppliers to declare one of the following, in relation to whether their product or service supports ODF.

(a) Yes, our application/solution can use ODF as its default format and complies in full and without any restrictions regarding any of the requirements around ODF.

(b) By using third party software, through a plugin or add-in, our application is able to read, create and revise documents according to the ODF 1.2 standard. If the end user selects ODF as its default format, he or she will have no restrictions on the functionality of our software based on an incomplete implementation. We are not aware of any loss of information that would occur to documents edited or reviewed by our solution, provided that they conform to the ODF 1.2 specification.

\(c\) Another (please ask supplier to provide details).

## Using free open source software based on ODF
The software you procure for working with editable documents must be compliant with ODF regardless of whether it is proprietary software (eg Microsoft Office) or free, open source software (eg LibreOffice). Downloading free software isn't considered procurement by European law if there's no service or support contract and you conform with the terms of use in the licence. Exceeding the licence's limits or procuring additional support and services such as training or development may involve a tender, depending on the value of the contract. In such cases normal procurement rules may apply.

You must still ensure that any free software you use supports ODF. See [Requirements](https://www.gov.uk/guidance/open-document-format-odf-guidance-for-uk-government/procuring-odf-solutions#core-requirements) for more information.

