---
layout: home-page
---

# The Octopus style guide

Everybody at Octopus writes whether it's documentation, blog posts, CLI help text, marketing copy, pitches, or text within the product itself. This guide aims to be a useful resource to serve as a quick reference to keep us consistent whenever we're unsure how to write a piece of text.

The style guide includes the following sections:

<ul>
{% for page in site.pages %}
  {% if page.title %}
    <li>
      <a href="{{ page.url | prepend: site.baseurl }} ">{{page.title}}</a>
    </li>
  {% endif %}
{% endfor %}
</ul>


## Contributing to the style guide

This guide is not intended to be an exhaustive resource that lists every possible way of doing something. Instead, it focuses getting people up and running as quickly as possible and as a place to add new insights as they occur.

The easy way to contribute to this guide is to raise a PR with the changes or additions you'd like to see added to the guide.
