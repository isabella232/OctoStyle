---
layout: page
title: Capitalization
order: 20
permalink: capitalization
family: language
---

As a general rule, capitalize words and terms that are proper nouns or would normally be capitalized. If you're uncertain, default to not capitalizing terms.

For Octopus, this means capitalizing product names, tool names, and the names of features, but not general concepts.

The following are capitalized when they refer to the product or product names:

- Octopus Server
- Octopus Cloud
- Workers
- Spaces
- Tentacles

The following are not capitalized (unless at the start of a sentence):

- deployment target
- environment
- server
- built-in repository
- runbooks (the concept not the feature)

## Proper nouns vs common nouns

A proper noun is the name of a specific instance of a thing, such as Australia and Octopus Deploy. A common noun is a general concept that refers to a class of things, such as country and deployment tool. The context words are used in can change whether a word is being used as a proper noun or a common noun. For instance,

> With the Octopus Spaces feature you can create separate spaces for each of your teams' infrastructure and projects.

In the above example, "Octopus Spaces" is the name of the feature, so it's capitalized, however, "separate spaces" refers to spaces as a general class of things and is not capitalized.

## Special note for IDs

There are a lot of IDs in the codebase, when referencing parameters in the code, match the casing in the codebase, i.e., 'ServerId', but when discussing the Server ID in the text, capitalize ID. (Id is a psychological term, ID is short for identification).

## Match the UI

The only exception to the rule is to use the same style as the UI you're documenting. For instance, deployment target is not a proper noun and should not normally be capitalized, however, if you are instructing a user to click a UI element in the Octopus Web Portal and the UI label is capitalized or all caps, you should mirror the style from the UI.

## Titles

Titles are written in sentence case, and only words that are normally capitalized are capitalized in titles.
