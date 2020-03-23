---
layout: page
title: Octopus snippets
---

This page lists the preferred naming conventions for Octopus specific terms and contains reusable snippets of text that can be included in your repo.



## Capitalization

As a general rule, capitalize words and terms that are proper nouns. If you're uncertain, default to not capitalizing terms.

In terms of Octopus this means capitalizing product names, tool names, and the names of features, but not general concepts.

The following are capitalized:

- Octopus Server
- Octopus Cloud
- Workers
- Spaces
- Operations Runbooks

The following are not capitalized (unless at the start of a sentence):

- Deployment target
- Environment 
- Server
- Built-in repository
- Runbooks (the concept as opposed to the feature)

## Snippets

The text snippets in this section are included from the [snippets repo](url). To include them in

### Octopus products

- Octopus Server 
    
    The Octopus Server (capitalized) is the product that on-premises customers download and install to access the REST API and the Octopus Web Portal. Do not use Octopus Deploy Server.

Short text snippet:

{% include snippets/octopus-server.include.md %}
    
- Octopus CLI

    The command-line tool for interacting with Octopus. Do not use Octo CLI.

## Octopus concepts

- Deployment targets 

    Deployment targets (not capitalized unless at the beginning of a sentence) are the servers, services, and accounts where users deploy their software.

