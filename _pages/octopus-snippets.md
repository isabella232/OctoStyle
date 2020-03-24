---
layout: page
title: Octopus snippets
---

This page lists the preferred naming conventions for Octopus specific terms and reusable snippets of text that can be included in your text.

## The snippets submodule

The text snippets on this page are included from the [snippets repo](https://github.com/OctopusDeploy/snippets) as a submodule that has [TODO] also been added to the docs and blog repos. 

### Add the snippets repo as a submodule to another repo

To add the snippets repo as a submodule to another repo, use the following command from the root of the repo, substitute `path/to/destination/directory` with the path to the directory where you want the snippets to be stored:

```
git submodules add https://github.com/OctopusDeploy/snippets path/to/destination/directory
```

### Update the snippets 

When the snippets repo is updated and you want to include the new snippets in your repo, do the following:

1. `cd` into the submodule, for instance, in the blog repository, the snippets submodule is located at: `blog/snippets/`:
1. Run `git fetch` to fetch the latest updates.
1. Run `git merge` to merge the updates.

## Snippets

To include the snippets in the blog, docs and any other repo where they are available, use the following syntax:

```
!include <snippet-name>
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

