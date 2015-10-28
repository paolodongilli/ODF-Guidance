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

# Validators and compliance testing
An overview of how validators and testing can ensure that applications dealing with editable documents are ODF-compliant.

## Reasons for compliance
You may need to use either 'validators' or software that compares applications to ensure they're compliant with ODF.

Software applications need consistency so that they can store, share and handle content that behaves in a way that a user expects. The ODF standard was designed to provide that consistency by defining a universal syntax (a shared 'formula') for producing documents.

Products that don't implement the standard correctly are bad for interoperability because they often create a poor user experience when documents are shared across different applications. Other applications then need to correctly deal with an increasing number of violations of the standard syntax. This is expensive and impractical to do now, but may be impossible in the future.

Compliance testing makes sure applications are built to the required standard.

## Use validators to test compliance
It's not possible to run a direct check against a productivity software application to see if it is built to a specific standard. You need to look at the output of applications, for example a text document or a spreadsheet. This can be done with a tool known as a 'validator'.

Validators are pieces of software that perform a series of automated tests to see if a document formally complies with a specification, in this case the ODF standard.

Validators produce a report that shows how a document does not conform to the specification, with a reasonable level of certainty. This helps give you an idea about whether the application (or combination of applications) used to produce the document conforms to the specification.

The ODF standard can be read by people in its text format, but is also produced in a [format that validator software can interpret](http://docs.oasis-open.org/office/v1.2/os/OpenDocument-v1.2-os-schema.rng) and that technical experts can use. This is rendered through another standard called [RelaxNG](http://relaxng.org/), a schema language. Validators can use this to automatically check a document against the standard to determine if it's compliant or not.

Not all checks can be machine-automated in a simple way. Some requirements will need additional dedicated programming to validate.

### Which validator to use
No single validator covers all conformance criteria of the ODF specification. There are many validators available that run complementary checks, so we recommend using several in parallel.

The OpenDoc Society has sponsored a free [online validator](http://validator.opendocumentformat.org/) based on the [ODF Toolkit](http://incubator.apache.org/odftoolkit/conformance/ODFValidator.html). Other downloadable validators include, for example, [Cyclone3](http://svn.cyclone3.org/branches/ODFValidator/) and [Office-o-Tron](https://code.google.com/p/officeotron/). You can also use one of the many [RelaxNG validators](http://relaxng.org/#validators).

The OpenDoc Society has more information about [downloading and using validators](http://plugtest.opendocsociety.org/doku.php?id=validators:installvalidator).

### Interpret the output of a validator
Validators produce detailed output from the tests they run, sometimes more than normal end users need. Validators aim to be as user-friendly as possible, but reading their results often requires some understanding of the standard.

You shouldn't automatically conclude from errors that are reported by a validator alone that a document does not conform to the specification. Equally, you shouldn't presume that a document conforms to ODF just because it appears to pass a validator test with no errors generated. Validators do not claim to be correct 100% of the time.

Issues highlighted by validators should still be investigated, however. It's important to run a set of representative documents through one or more validators. Reviewing the output will help you understand the level of standards support across the range of applications that were used to create and manage those documents.

## Use comparison software to test compliance
Comparing how documents are handled in different applications is an alternative to validators for testing application compliance.

Officeshots is a convenient tool for this. It's a collaborative effort of the OpenDoc Society and the government of the Netherlands, and is available as a [free online service](http://www.officeshots.org/) and as an [open source tool](http://code.officeshots.org/trac/officeshots).

If you're considering a particular application, Officeshots can provide an initial but thorough check to see it handles ODF in the way it claims to. It allows you to compare the output and behaviour of a variety of applications, based on documents that are relevant to your organisation rather than on a synthetic benchmark. For instance, do the templates produced by your communications department or design agency look consistent across all the applications they are likely to be used in? How do your outgoing letters look if you view or print them in EuroOffice 2014, different versions of Microsoft Office or Google Docs?

The documents you provide to Officeshots as input, as well as the results from passing these documents to the different applications, are checked in a number of validators automatically. The resulting documents and the validator results can be downloaded, for more thorough evaluation or bug analysis.

Officeshots can run automatically on sets of test documents (ie test suites), or works with other testing methods such as the [ODF autotests](https://github.com/vandenoever/odfautotests).

[Source code and documentation](http://code.officeshots.org/) are available, as are [sets of test documents](http://officeshots.org/galleries).

