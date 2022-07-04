---
layout: home-page
description: Style info
---

Everybody at Octopus writes whether it's documentation, blog posts, CLI help text, marketing copy, pitches, support emails, or text within the product itself. This guide is a quick reference for the conventions we use at Octopus, and a resource to keep us consistent whenever we're unsure how to write or structure a piece of text.

The style guide includes the following sections:

<ul>
{% assign pages = site.pages | sort: "order" %}
{% for page in pages %}
  {% if page.title != home %}
    <li>
      <a href="{{ page.url | prepend: site.baseurl }} ">{{page.title}}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>

## Contribute to the style guide

The easiest way to contribute to this guide is to raise a PR in the [repo](https://github.com/OctopusDeploy/OctoStyle) with the changes or additions you'd like to see added to the guide.

This guide is a simple [Jekyll](https://jekyllrb.com/) site. The main content pages are written in [Markdown](markdown.md) and are located in the `_pages` directory.