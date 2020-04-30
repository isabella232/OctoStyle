---
layout: page
title: The snippets submodule
order: 55
permalink: snippets-submodule
family: snippets
---

The [Octopus snippets](octopus-snippets.md) are included from the [snippets repo](https://github.com/OctopusDeploy/snippets) as a submodule that has also been added to the docs and blog (temporarily disabled for the blog) repos. 

### Add the snippets repo as a submodule to another repo

To add the snippets repo as a submodule to another repo, use the following command from the root of the repo, substitute `path/to/destination/directory` with the path to the directory where you want the snippets to be stored:

```
git submodules add https://github.com/OctopusDeploy/snippets path/to/destination/directory
```

### Update the snippets 

When the snippets repo is updated and you want to include new snippets in your repo, do the following:

1. `cd` into the submodule, for instance, in the blog repository, the snippets submodule is located at: `blog/snippets/`:
1. Run `git fetch` to fetch the latest updates.
1. Run `git merge` to merge the updates.
