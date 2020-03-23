---
layout: page
title: Octopus snippets
---

This page lists the preferred naming conventions for Octopus specific terms and contains reusable snippets of text that can be included in your repo.

## Snippets

The text snippets in this section are included from the [snippets repo](https://github.com/OctopusDeploy/snippets). To include the snippets in the blog and the docs use the following syntax:

```
!include <snippet name>
```

## Octopus Server 
    
    The Octopus Server (capitalized) is the product that on-premises customers download and install to access the REST API and the Octopus Web Portal. Do not use Octopus Deploy Server.

Short text snippet:

`!include <octopus-server>`

{% include snippets/octopus-server.include.md %}
    
## Octopus CLI

    The command-line tool for interacting with Octopus. Do not use Octo CLI.

## Deployment targets 

    Deployment targets (not capitalized unless at the beginning of a sentence) are the servers, services, and accounts where users deploy their software.

