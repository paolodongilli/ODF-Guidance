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

# Avoid macros in documents
Why macros shouldn't be used in documents and what alternatives ODF can offer.

## What macros are
Macros are small pieces of software included within a document to automate certain repetitive tasks, such as alphabetically sorting items in a bulleted list.

Macros offer features that make them both convenient and powerful, but they also have problems with interoperability and security. Macros that work on one version of software or platform won't necessarily function on another. They can also allow viruses to infect your computer and distribute themselves using an application's own programming language. Even when a file comes from a known and trusted person or organisation it may already be infected without their knowledge.

For these reasons the UK government forbids the use of macros in publicly shared documents and advises against their use in general.

## Alternatives to macros
Web-based document solutions provide the same interactive and automatic functions as macros do, but without the interoperability and security issues.

Office applications can nearly always offer the same functions as macros through extensions, add-ons and plugins. If the right one doesn't exist, you can get one built.

Before using extensions, add-ons or plugins you should:

- test them for interoperability and usability to make sure there are no unintended side effects when you share documents across platforms
- get them vetted by IT security professionals
- restrict levels of access for certain privileges to developers or system administrators (give users content-level access only)

## Assess your organisation's macros
Before you look for an alternative to a specific macro you should first determine if it's meeting a user need.

First run an automated scan for macros on system drives. You may discover that many macros are undocumented, quick workarounds created by a user to complete a one-off task. There may also be more than one macro created by different users but for the same purpose. Recreating most of these macros as a plugin would not be worth the cost.

You should also ask your users what functions they would be missing if document macros are disabled. Ask them to list those macros they actually use. One German government agency counted 9,000 macros on disk but found that users only needed 9.

## Plan your move away from macros
Moving your organisation to open file formats gives you a good opportunity to assess and improve its processes related to documents.

Start to determine how widespread macros are in your organisation and what functions they provide. If macros are widely used don't try to stop using them all at the same time. If something goes wrong during this kind of 'big bang' approach, your users might be confused about what is causing the issue.

Once you have an overview of which macro functions need to be recreated in plugins or applications, begin planning the order in which you'll turn off document embedded macros. You should also work out a budget for doing so and involve IT security staff to make sure you understand related security issues.

## Deal with macros post-migration
To prevent your users from unintentionally using macros, disable them in the settings for all applications. You may also be able to scan incoming documents and remove macros before they reach the user.

If your staff can't avoid using macro-embedded documents at first, provide a standalone (preferably offline) machine where users can take macro-embedded documents on a thumb drive and process them in isolation from other systems.

