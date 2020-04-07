---
layout: page
title: Writing for Octopus TL;DR
order: 0
permalink: writing-at-octopus-tldr
---

This pages includes the basics you need to get started, as does the [basic blog template](https://github.com/OctopusDeploy/blog/blob/master/templates/basic-template.md). More detailed instructions are available in the rest of this guide.

## Markdown

The blog and the docs are both written with [markdown](markdown.md).

The following is the minimum markdown you need:

1. `## H2 Heading, ### H3 heading.`

1. Use `**bold**` for feature names and UI elements, use `*italics*` to add emphasis, and use back ticks for parameters and file paths:
~~~
`~/.ssh/id_rsa.pub`
~~~

1. Add `[links](https://www.octopus.com)`.

1. Code blocks:
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

Use sentence case for titles. Sentence case uses the same capitalization rules as normal sentences. Title case capitalizes most words in the title, but we don't use title case.

## Images

Use images and screenshots to help illustrate your point. Here are some pointers for images see [working with images](images.md):

   1. Crop the image so only the window you’re showing is visible.
   1. Show enough of the UI that readers can see where they need to look, but don’t include the entire screen if it’s not needed.
   1. Use screenshots to reassure readers they're on the right path, but don't use screenshots for ever step users need to take.
   1. Resize your images so they’re 72dpi.
   1. Don’t rely on the image alone to explain steps a user must take. If there is information in the screenshot the user needs, repeat it in the text (screenshots go stay and users can't copy and paste from screenshots).
   1. If your screenshot is of the Octopus UI, use light mode.

## Proofread

Proofread your work to make sure it's error free and validates with Docsync. Octopus has a Grammarly account that anybody can use that can help with this.

## Create a PR

When your work is ready, create a PR so the work can be reviewed, edited, scheduled (if it's for the blog) and merged.