---
layout: page
title: Writing documentation quick start 
order: 35
family: language
---

The purpose of documentation is to help the user understand the tool they are using and overcome any blockers that are preventing them from reaching their goal.

The Octopus Deploy documentation lives at [octopus.com/docs](https:www.octopus.com/docs), and is stored in the [GitHub repo](https://github.com/OctopusDeploy/docs).

The following pages provide additional information about writing at Octopus and are recommended reading before continuing with this page:

- [Writing for Octopus TL;DR](/writing-for-octopus-tldr.md)
- [Markdown quick reference](/markdown.md)
- [Voice and style](/voice-and-style.md)
- [Working with images](/images.md)

## How to structure content

You should structure documentation as follows:

1. Introduction.

   Provide an introduction that explains what the documentation covers and provide some sample scenarios that highlight the main use cases for the feature being documented.

   **Note**: Edge cases should be included in the reference/advance use cases section at the end. Avoid adding edge cases to the main body of the text as they can confuse people about the intended purpose of the feature.

2. Procedural.

   Next, provide the information the user needs to successfully use the feature. Where ever possible, break the procedure into simple step-by-step instructions to make it as easy as possible for the user to follow:

   > 1. Select **Projects** from the main navigation in the Octopus Web Portal, and click **ADD PROJECT**.
   > 2. Give the project a name that's meaningful to you and anybody else who'll work on the project.
   > 3. ...

3. Additional information

    Next, provide any reference material, advanced uses cases or edges, troubleshooting steps, and FAQs.

   **Reference material**

    Tables provide an easy way for users to scan lists parameters of parameters for the ones they need. If the reference material is extensive, add it to a child page and link to it.

    If there are common troubleshooting steps users might need to perform, list them here.

4. Learn more

    Add links to related documentation, the blog, or other resources to help the reader continue their journey.

## Adding new page vs. editing an old page

As a rule of thumb, we should aspire to make each explain something that will help the reader achieve a goal.

In some scenarios, there might be multiple options and including them all on a single page might give the reader scroll fatigue or make it difficult to jump between the pieces they need. In such cases, it might be better to include the options on child pages.

