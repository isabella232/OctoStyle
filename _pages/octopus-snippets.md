---
layout: page
title: Octopus snippets
order: 50
---

This page lists the preferred naming conventions for Octopus specific terms and reusable snippets of text that can be included in the blog, the docs, or any other repo that has [added the snippets repo as a submodule](snippets-submodule.md).

To include specific snippet text, use the following syntax:

```
!include <snippet-name>
```

There are four types of snippets:

- One line: A brief sentence that states what something is but doesn't provide any context.
- short: 
- Full: 
- Extended:

{% for term in site.terms %}
## {{ term.description }}
	{% if term.notes %}
{{ term.notes }}
	{% endif %}
	{% if term.one-liner == true %}
		{% assign one-liner = term.handle | append: "-one-line.include.md" | prepend: "snippets/" %}

**One line snippet**:

To include, use: 

`!include <{{ term.handle | append: "-one-line" }}>`

{% include {{ one-liner }} %}
	{% endif %}
		{% if term.short == true %}
		{% assign short = term.handle | append: "-short.include.md" | prepend: "snippets/" %}
**Short snippet**:

To include, use: 

`!include <{{ term.handle | append: "-short" }}>`

{% include {{ short }} %}
	{% endif %}
{% endfor %}
    
## Deployment targets

 Deployment targets (not capitalized unless at the beginning of a sentence) are the servers, services, and accounts where users deploy their software.

