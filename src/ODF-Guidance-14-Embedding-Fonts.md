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

# Embed fonts in ODF documents
How to embed fonts in ODF documents, and guidance on choosing fonts.

## Open licence fonts
To help ensure documents look the same to all viewers no matter what device or platform they're using, always embed any specific fonts used to compose them.

Open Document Format (ODF) lets you embed fonts inside any document. To make the most of this feature, you should use fonts with an open licence as the default fonts in your applications.

The benefits of 'open fonts' are that they help you:

- reduce costs (some fonts can be very expensive to install and license for each user)
- avoid documents being inaccessible or 'broken' to some users because of licence restrictions
- avoid legal compliance problems
- have more control over how your documents look to all users
- keep more accessible archives

You can get open fonts from:

- most Linux/UNIX distributions such as [Debian](https://www.debian.org/), [Fedora](https://getfedora.org/), [OpenSuse](https://www.opensuse.org/en/) and [PC-BSD](http://www.pcbsd.org/)
- many open source office applications
- non-commercial open font resources such as [Open Font Library](http://openfontlibrary.org/) project and [CTAN](https://www.ctan.org/tex-archive/fonts?lang=en)
- [Google Fonts](https://www.google.com/fonts)

Whether you use open or restricted fonts, you need to set a clear policy on which fonts you use and make it available to users.

## Freeware and shareware fonts
Freeware and shareware fonts are also available online. These are usually distributed for free but their creator expects a payment when you start using them for business purposes.

They may or may not be safe to embed and modification (eg to accommodate adding a new currency glyph or diacritics) probably won't be allowed.

If you want to use a freeware or shareware font because you can't find a similar open font, you should first check its licensing conditions. These can usually be found online.

## Microsoft and Windows fonts
Some font files are restricted by specific commercial licences. For example:

- the default typeface used in the recent versions of Microsoft Office - the sans-serif typeface Calibri
- fonts distributed alongside the latest versions of Windows and Microsoft Office - such as Cambria, Candara, Consolas, Constantia and Corbel

These ClearType Font Collection fonts pose significant problems to users on other platforms, including most smartphones and tablets.

So if you're using these fonts you should embed them (embedding is allowed according to the licensing information Microsoft has published on its site).

You can't embed the Microsoft fonts Arial, Arial Narrow, Times New Roman, or Courier New.

### Check if you can embed Microsoft and Windows fonts
For Windows users there is a free tool called [font properties editor](https://www.microsoft.com/typography/property/fpedit.htm) that allows users to check if a particular font can be embedded. This check is based on the information stored within the fonts themselves.

For fonts produced by Microsoft itself, you can also consult the website of [Microsoft Typography](https://www.microsoft.com/en-us/Typography/default.aspx) for licensing information and how to check compliance.

### Alternative open fonts
Many fonts can be used for embedding without any issue:

- the open font [Carlito](http://openfontlibrary.org/en/font/carlito) is a sans-serif font that can be used as a drop-in replacement (ie font-metric compatible) for Calibri and can also be used online
- the [Caladea](http://openfontlibrary.org/en/font/caladea) open font is metrically compatible with Cambria
- the so-called [Liberation fonts](https://fedorahosted.org/liberation-fonts/) can be used to replace the previous generation of fonts used by Microsoft: Arial, Arial Narrow, Times New Roman, and Courier New

## Add a font manually
ODF lets you embed fonts 'as is', meaning that technically the entire font file is put inside the document without making any changes to it. This allows a user to take an embedded font and install it on their system. ODF places no restriction on the user to embed or use any font, and leaves it entirely up to the user to deal with this capability responsibly and legally.

You can embed fonts manually by following a few simple steps or by using Fontos, a handy open source tool that allows you to see what fonts your documents are using and to drag and drop them using a web browser.

