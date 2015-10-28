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

# ODF spreadsheets and formulas
Important considerations when working with spreadsheets and formulas in ODF.

## OpenFormula for data manipulation
Spreadsheets perform many functions for users, from repetitive calculation tasks on ranges of data to storing and sorting ranges of text information. They offer a simple data entry and lightweight programming environment that allows users who lack programming knowledge to perform simple data manipulation tasks.

OpenDocument Format 1.2 includes OpenFormula, a standardised set of formulas that should be present in every compliant application. Formulas are small software routines in spreadsheets that allow users to perform tasks. They allow a combination of:

- fixed parameters, text strings and logic operators
- data (ranges) from elsewhere within the spreadsheet or its metadata
- (selection of data from) another source such as a database
- the result of the computation of other formulas

Because OpenFormula operates across all Open Document Format (ODF) applications, when you cut and paste part of a spreadsheet into a document, it will retain the actual logic behind the cell values rather than just copy their context as text or image.

Using OpenFormula also prevents different formulas with identical names from being confused when users operate between different proprietary spreadsheets. No special converters or compatibility modes are needed. Versions of the standard before ODF 1.2 may still have issues when interacting with Microsoft Excel or other spreadsheets, so be sure to update to the most current version of the standard.

## Levels of OpenFormula implementation
OpenFormula can be implemented at 4 different levels, each offering progressively more capability:

- minimum: providing the minimal capabilities (including functions, types, and their meanings) that are very widely implemented with spreadsheet applications, even in resource-constrained environments (this includes about 100 functions)
- minimum desktop: providing the minimal capabilities expected from typical desktop spreadsheets
- basic: providing all the capabilities necessary for typical desktop spreadsheet use (adds a distinguished logical type and support for complex numbers)
- full: providing some additional, less-commonly used features intended for advanced users

The minimum and minimum desktop levels provide all the functionality the vast majority of users will require. They're widely implemented by desktop spreadsheet applications.

When implemented at the basic level, an application supports all the functions supported by equivalents like Microsoft Excel.

Apart from the extended range of formulas, basic and full implementations have some provisions for backwards compliance with older application-specific issues. Since not every application is likely or expected to support all these levels, it might be better to properly convert the formulas in your spreadsheets so they don't depend on such backward compliance features.

## Problems converting spreadsheets to ODF
ODF 1.2 has been extensively tested by many experts from a variety of backgrounds. Conversion problems are most likely to be the result of historical product features being improperly mapped to the ODF standard.

Software sometimes strips out some functionality during the conversion. For instance Excel spreadsheets converted into OpenDocument Format 1.1 using Microsoft Office may not display drop-down lists. Some of the differences between historical application defined formats are small but can still cause significant problems.

A few are highlighted in the annotated version of the OpenFormula specification, which also provides useful background information.

Some vendors provide an overview of their design choices when implementing ODF; these notes (such as the implementation of ODF in Microsoft Excel) can provide additional clues. If you experience problems with conversion, follow these steps.

1. Test a more recent software version to see if the issue has been addressed.
2. Check if there are plugins or add-ins that might solve the problem.
3. Ask your vendor why it doesn't work and ask when the function can be restored.
4. If you can't wait, consider getting support to improve the product or build a plugin or add-on.
5. Alternatively, select a different desktop publishing tool that does meet your needs.

## Known issues
### Precedence issue
To give accurate outcomes to formulas, spreadsheets need to assign precedence (priority) to different mathematical operators. Precedence varies between products, which can cause issues.

In OpenFormula, prefix '-' is given a higher precedence than '^', to accommodate that '-2^2' remains '4' in Microsoft Excel and products that aimed to be compatible with it, such as OpenOffice, LibreOffice and Gnumeric. Because prefix '-' had a lower precedence in Lotus 1-2-3, Quattro Pro, and Excel's own Visual Basic, these products need to insert and remove parentheses when reading/writing expressions in OpenFormula where this matters.

### Decimal separators
In a formula, to distinguish between subsequent parameters, OpenFormula uses the semicolon ';'. Many locations that don't use US English use the comma ',' as the decimal separator. Using the semicolon as the parameter separator eliminates confusion and the risk of incorrect implementation. Excel traditionally uses the comma as the function parameter separator, which may cause incorrect usage.

### Empty parameters
In normal circumstances, OpenFormula does not allow empty parameters in formulas. By setting the application to behave according to the Basic level of implementation, that application can emulate the behaviour of Microsoft Excel to accept empty parameters in any position. Typical implementations will have many built-in functions, and most implementations also support one or more ways to create user-defined functions.

### Workarounds to Excel AND/ OR bug
Microsoft Excel's AND and OR functions historically did not work correctly in array formulas. This is a known bug. OpenFormula provides a correct definition of these functions. The traditional workarounds as recommended by some literature (using * and + inside array formulas as a work around) should however still work in ODF.

### Intersection operators
In Microsoft Excel's display format, the space is used as the intersection operator. This can easily lead to mistakes or be confusing at the least. The OpenFormula exchange format uses '!' instead for intersection.

