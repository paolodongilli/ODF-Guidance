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

# Platforms and devices
An overview of the platforms and devices that work with ODF, as well as security and accessibility considerations.

## Operating systems
The Open Document Format (ODF) standard has been implemented on nearly all operating systems for desktops, laptops, mobile phones and tablets, including:

- Android (with many derivatives)
- Apple iOS
- Apple OS X
- Blackberry/QNX
- Chromium OS
- DragonFlyBSD
- eComStation
- Firefox OS
- FreeBSD
- GNU/Linux
- GNU/Hurd
- the Maemo, Mer and Sailfish family of mobile OS
- Microsoft Windows
- Microsoft Windows phone
- NetBSD
- OLPC
- OpenBSD
- OpenIndiana
- Plasma Active
- ReactOS
- Solaris
- Ubuntu touch

## Web-based solutions

Users can also work with the ODF standard through a web platform. This allows ODF to be used on nearly every smartphone, feature phone and tablet currently on the market.

There are 2 classes of solutions based on web technology:

- server-based office applications with a web front-end
- in-browser solutions

Server-based web office applications (such as OX Office, Google Docs, Office 365 and Zoho Office) translate the documents on the server into HTML or another format which can be viewed with a web browser.

In-browser solutions (such as those based on the open source WebODF library) are self-contained and do not require any installation or full internet access. In terms of security and privacy, in-browser solutions are most similar to traditional installed software because:

the actual document is shown and edited directly on the end user device
network connectivity isn't required to edit or view documents (only for collaborative working)
once the web viewer or editor is downloaded to the browser, there aren't dependencies on software running somewhere else
In-browser solutions for viewing and editing ODF can be served alongside the document from environments such as:

- your website
- intranets
- extranets
- content management systems
- document repositories
- webmail

Your organisation can also choose to package an in-browser solution as a native or web app for a phone, or attach an add-in or extension to the browser. Running it from a local copy is much more secure and prevents data loss if you lose your internet connection. The main downside is you need to remember to download updates.

## Security on platforms and devices
Many solutions for different platforms and devices won't offer the necessary security for working with confidential or sensitive documents. Where higher security is required this can be met with:

- locally installed software (including apps) without remote components
- in-browser solutions
- solutions based on a self-hosted web server (ie not accessed through the internet)

When using locally installed software, devices don't need to be connected to offer full document functionality. Local solutions also allow users to automatically apply strong encryption before saving a document (locally or remotely) or synchronising with their cloud provider. Server-based solutions are viable where users always have a reliable network connection and where the server is hosted in a trusted environment.

### Connectivity requests
If any software you're evaluating asks for generic permission to connect to the internet you should investigate why it's doing this. Don't assume an application just needs a network connection to display advertisements, unless you've first made sure that your content is secure.

Some software interacts automatically with untrusted remote destinations. For example, many mobile apps for both iOS and Android need to send a document to a remote server in order to convert it from one format to another. This can also pose a security risk.

If you're working with confidential or sensitive documents and require a secure solution you should:

- thoroughly audit the solutions you already use
- inspect the source code of solutions before adopting them (or, preferably, compile it yourself)
- make sure the devices you use offer adequate security
- review any software that's been updated by someone else (e.g. someone maintaining an app store)

See the chapter in this manual on privacy and security (Section 8 - Privacy and security) for more information.

## Accessibility on devices with alternative input
Until relatively recently office applications were used almost exclusively on desktops and laptops, which use larger displays and traditional input devices like a mouse and keyboard. Disabled users have been able to use office applications through accessibility features designed for these systems, often through third-party solutions.

Many smartphones, tablets and other devices use touch-screen technology, which poses new challenges to making documents fully accessible. There are particular challenges for people with impaired visual or motor abilities, in terms of both user interaction and overall user experience.

In-browser solutions can offer increased accessibility, particularly if they're created following the W3C's recommendations for authoring tools. Browser-based solutions are vendor-neutral in terms of the hardware they use - an attractive feature if you don't control the hardware your users use or don't want to be locked into a specific platform.

Some applications are highly optimised for intricate touch usage and are difficult to make accessible. For these it might be worth considering standalone alternatives.

See the chapter on accessibility (Section 7 - Accessibility) for more information.

## Developing platform or device-specific solutions
If you need a solution for a class of devices or a specific platform and none of the existing solutions fit all of your user needs, you could consider developing a custom solution. From a legal perspective, there are no known restrictions in software patents to stop you from implementing the ODF standard on any platform or device or in open source software. You can also adapt open source solutions that are already close to meeting your requirements.

If software or an app exists for another platform there's also the option to port a version to the platform you're using. Existing open source software applications centered around ODF have already been ported to many different platforms. This includes complete open source touch-enabled solutions that can run on tablets and smartphones, such as those based on the [Calligra](https://www.calligra.org/) project.

The technical specifications of ODF are available online for free and there are dozens of software libraries in many programming languages available to work with ODF. OpenDoc Society provides an extensive repository of [example code](http://recipes.opendocsociety.org/) ready for free reuse.

Most open source projects are eager to work on new features, and many organisations find that the cost for hiring people to develop the features they need is quite low compared to the total cost of ownership of office applications.

If you currently use a non-open source solution on one platform and need to add more features, contact your vendor and let them know what you want. If they are unable to supply these features, consider creating a plugin, extension or add-on to meet your need.

