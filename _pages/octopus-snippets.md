---
layout: page
title: Octopus snippets
---

This page lists the preferred naming conventions for Octopus specific terms and reusable snippets of text that can be included in the blog, the docs, or any other repo that has [added the snippets submodule](snippets-submodule.md).

To include specific snippet text, use the following syntax:

```
!include <snippet-name>
```

## Octopus Server (capitalized)
    
The Octopus Server (capitalized) is the product that on-premises customers download and install to access the REST API and the Octopus Web Portal. Do not use Octopus Deploy Server.

One line text snippet:

`!include <octopus-server-one-line>`

{% include snippets/octopus-server-one-line.include.md %}

Short text snippet:

`!include <octopus-server-short>`

{% include snippets/octopus-server-short.include.md %}
    
## Octopus CLI

The command-line tool for interacting with Octopus. Do not use Octo CLI.

## Deployment targets 

 Deployment targets (not capitalized unless at the beginning of a sentence) are the servers, services, and accounts where users deploy their software.

