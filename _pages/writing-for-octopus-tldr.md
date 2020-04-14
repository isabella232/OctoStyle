---
layout: page
title: Writing for Octopus TL;DR
order: 0
permalink: writing-at-octopus-tldr
family: language
---

This pages includes the basics you need to get started, as does the [basic blog template](https://github.com/OctopusDeploy/blog/blob/master/templates/basic-template.md). More detailed instructions are available in the rest of this [guide](https://octopusdeploy.github.io/OctoStyle/).

## Markdown

The blog and the docs are both written with [Markdown](markdown.md).

The following is the minimum Markdown you need:

1. `##` H2 Heading, `###` H3 heading.

1. Use `**bold**` for feature names and UI elements, use `*italics*` to add emphasis, and use back ticks for parameters and file paths:
~~~
`~/.ssh/id_rsa.pub`
~~~

1. Add a `[link](https://www.octopus.com)`.

1. Create a code block:
~~~
```
Write-Host "Hello, World!"
```
~~~

1. Add an image: 
~~~
![Description of the image](image-name.png "width=500px")
~~~

## Sentence case

Use sentence case for titles. Sentence case uses the same capitalization rules as normal sentences, whereas title case capitalizes most words in the title. We don't use title case.

## Images

Use images and screenshots to help illustrate your point, but don't rely on images alone to convey your meaning. Use a screenshot if:

- They might struggle to locate an item in the UI.
- The procedure jumps from one place in the UI to another.
- You want to reassure them they’re in the right place.

For more information see [working with images](images.md).

## Proofread

Proofread your work to make sure it's error free and validates with Docsync. Octopus has a Grammarly account that anybody can use that can help with this.

## Create a PR

When your work is ready, create a PR so the work can be reviewed, edited, scheduled (if it's for the blog) and merged.
