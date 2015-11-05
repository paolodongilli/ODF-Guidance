# Open Document Format (ODF): A Guidance for Governments

The present document in its initial release doesn't bring anything more, in terms of content, to the original ODF guidance from the Cabinet Office of the UK Government acknowledged below. 

The need of a fork was mainly meant to render the document in a textual format (Pandoc's Markdown) in order to be able to store it onto a public repository (GitHub) and easily keep track of versions and changes.
The original guidance is available in HTML format only, accessible by means of copy and paste from the UK Government web pages. 

I thought the document had to be a general guidance for any government interested in adopting ODF as the world's leading open document standard. 

Generalizing it, rendering it into Markdown and committing it onto GitHub will allow people to join the effort to keep it up-to-date, correct typos, add new content and easily fork it e.g. for translation purposes.

## Converting the files into another format

For converting the source of this document from Markdown format into other formats (e.g. ODF, PDF, HTML, ...), I suggest [Pandoc](http://pandoc.org/), a universal free software document converter available under the GPLv3 license.

### Usage

I suppose you have [Git](https://git-scm.com/) and [Pandoc](http://pandoc.org/) installed (with their respective dependencies) and accessible through a shell.

1. Download the `ODF-Guidance` folder from GitHub. The directory contains this README file, a `src` directory containing a Markdown (.md) file for each chapter of the document; a `templates` folder containing the LaTeX and ODT templates which are slightly modified versions of the ones offered by Pandoc; an `output` directory containing some conversion samples.

> ```$ git clone https://github.com/paolodongilli/ODF-Guidance.git```

2. Move into the ODF-Guidance directory:

> ```$ cd ODF-Guidance/```

3. Convert the document source in two sample outputs

  * Create the PDF version of the document (LaTeX needs to be available on your system):

> ```$ pandoc --template=templates/latex.template --toc --number-sections -o output/ODF-Guidance.pdf src/*.md```

  * Create the ODF (.odt) version of the document: 

> ```$ pandoc --template=templates/odt.template --reference-odt=templates/reference.odt --toc --number-sections -o output/ODF-Guidance.odt src/*.md```   


## Copyright Notice and Licensing Terms

Copyright (C) 2015 Crown Copyright 

Copyright (C) 2015 Paolo Dongilli

This document is licensed under the [Open Government Licence v3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

## List of Contributors

- Cabinet Office, UK Government
- Paolo Dongilli, Autonomous Province of Bozen-Bolzano, South Tyrol, Italy
- ADD YOUR NAME HERE

## Acknowledgements

The current document is a slightly revised version of the document "Open Document Format (ODF): guidance for UK government" released by the Cabinet Office of the UK Government as of 11 September 2015. The original document can be found here [https://www.gov.uk/guidance/open-document-format-odf-guidance-for-uk-government](https://www.gov.uk/guidance/open-document-format-odf-guidance-for-uk-government), licensed under the [Open Government Licence v3.0](http://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).

