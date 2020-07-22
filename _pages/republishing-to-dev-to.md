---
layout: page
title: Republishing to dev.to
permalink: republish-dev-to
order: 70
family: language
---

Sometimes we want to republish blog posts to the Octopus account on [dev.to](https://dev.to/octopus/). However, some of the techniques used in this style guide, and therefore our posts, aren't supported in dev.to. There are a number of steps you can take to ensure a smooth migration for your post. This section outlines a step-by-step guide to republish an article to dev.to.

1. Choose the article you want to republish and find its markdown page in GitHub.

   Select the markdown page for the article (it's usually `index.md`). In GitHub, choose the **Raw** contents of the file, and copy everything to your system clipboard - including the headers at the top of the page.

1. Copy the article content into a new post in dev.to 

   On the dev.to site, choose **Write a post** in the top-right corner of the page. Remember to switch the drop-down of *write a new post* from **Personal** to **Octopus** (this can be done later so don't worry if you forget). 
   
   Next, copy the contents of the clipboard below the dev.to header information:

   <img src="{{site.url }}/assets/img/republishing-post-copy-content.png" />

1. Edit the dev.to post header.

   > This guide assumes you are using the basic markdown editor, but you can choose to use the rich-markdown editor by switching to that in the dev.to UX settings section.

   The header for articles in dev.to are similar to ones used on the Octopus blog. Fill out the following:

   - `title` - this can be copied from the existing post.
   - `published` - this can be left as `false` while you are editing, and then switch the value to `true` when you are happy with the post.
   - `description` - this can be copied from the existing post.
   - `tags` - these are a comma separated list in dev.to, and while they may match some of the Octopus tags, it's worth doing some homework to find which ones are appropriate for the post. Some sensible tags are likely to be:
     - octopus
     - devops
     - deployment
   - `cover_image` - you can use the **Upload image** option at the top of the editor to upload the main image from the existing post, or preferably provide the full UrL from octopus.com. For example:

      ```yml
      cover_image: https://i.octopus.com/blog/2020-01/ultimate-guide-to-rolling-deployments/rolling-deployments.png
      ```
   
   In addition to these, add the following new header item:
   - `canonical_url` - this is the URL from octopus.com which dev.to will add to the top of the republished post to link back to the original post.

1. Remove the original post's header information.

   After you have edited the new post's header, you can remove the existing one. Optionally, remove the main octopus.com image which is typically at the top of the original post too. This prevents having the same image appear twice in quick succession:

   <img src="{{site.url }}/assets/img/republishing-post-remove-header-image.png" />

1. Use the dev.to review option while editing.

   It's useful to keep checking what the republished post will look like. Switching between this and the editor is a good way to check the post looks the way you expect.

1. Upload any images, or change markdown and image links to full URL paths.

   Any images from the original post won't resolve in dev.to unless you upload them. Preferably, look for any image files in the markdown and change them to their full path. For example:

   ```md
   ![Project sequential deployment process](project-sequential-deployment-process.png)
   ```

   Becomes:

   ```md
   ![Project sequential deployment process](https://i.octopus.com/blog/2020-07/convert-to-rolling-deployments/project-sequential-deployment-process.png)
   ```

   For the same reason, any links to other blog posts where you use the relative path to a markdown file should also be modified to the full URL path.

1. Remove or change hints, warnings, error, and success callouts.

   Posts on octopus.com which make use of any of the following callouts won't work on dev.to:
   - hint
   - warning
   - error
   - success

   The simplest option is simply to remove them. Alternatively, you can edit the post and add a markdown block-quote. For example:

   ```md
   > This text will appear as a block quote.
   ```

   Which is rendered as:

   > This text will appear as a block quote.

1. Remove any use navigation paths using the `{{Navigate>Here}}` syntax.

   Navigation paths in dev.to won't work. For example, if you kept the following syntax:

   ```md
   Go to the runbook process from the {{Operations>Runbooks}} section. 
   ```

   The preview editor in dev.to will complain that Liquid variables aren't enabled.

   The simplest thing to do is to convert them manually. In the example above it would look like this:

    ```md
    Go to the runbook process from the Operations ➜ Runbooks section.
    ```
    
   This will render as:

   Go to the runbook process from the Operations ➜ Runbooks section.


1. Remove the `!toc` from the start of the post.

   Posts on octopus.com which make use of the `!toc` (table of contents) markdown won't work on dev.to.

   The simplest option is to remove this markdown. For longer posts (for example *ultimate guides to X*) it can be beneficial to manually add a table of contents using a mix of standard markdown and HTML.

   If you wish to include this, add a header and a bullet point list of the main sections you want to highlight. For example:

   ```md
   ## In this post
   * [The application](#the-application)
   * [Sequential deployment process](#sequential-deployments)
   * [Convert to a rolling deployment process](#convert-to-rolling-deployment)
     * [Scale up the servers](#scale-up-the-servers)
     * [Choosing a load balancer](#choosing-a-load-balancer)
     * [Load balancer target pools](#load-balancer-target-pools)
     * [Create a new project](#create-a-new-project)
     * [Convert the PetClinic deployment process](#convert-the-petclinic-deployment-process)
     * [Switch over to new infrastructure](#switch-over-to-new-infrastructure)
     * [Clean-up](#clean-up)
   * [Conclusion](#conclusion)
   ```

   which is rendered as:

   ## In this post
   * [The application](#the-application)
   * [Sequential deployment process](#sequential-deployments)
   * [Convert to a rolling deployment process](#convert-to-rolling-deployment)
     * [Scale up the servers](#scale-up-the-servers)
     * [Choosing a load balancer](#choosing-a-load-balancer)
     * [Load balancer target pools](#load-balancer-target-pools)
     * [Create a new project](#create-a-new-project)
     * [Convert the PetClinic deployment process](#convert-the-petclinic-deployment-process)
     * [Switch over to new infrastructure](#switch-over-to-new-infrastructure)
     * [Clean-up](#clean-up)
   * [Conclusion](#conclusion)

   Next, add the links to the headers of each section using an `<a>` HTML hyperlink tag. For example, for the `The application` header, you need to change it from:
   
   ```md
   ## The application
   ```
   To the following:

   ```md
   ## The application <a name="the-application"></a>
   ```

1. Review the post for any newline characters between number or bulleted-lists.

   It appears that dev.to is less forgiving than octopus.com when there are any newline characters present between number or bulleted lists. Usually, removing the offending newline CR;LF characters corrects this.

1. Optionally, add an original post link to the end of the post.

   This tends to be personal preference, but it's usually a good idea to add the following markdown to the end of the republished post:

    ```md
   _This post was originally published at [octopus.com](https://link-to-the-octopus-com-post)._
    ```
   where `https://link-to-the-octopus-com-post` is the canonical URL of the post being republished.

1. Publish your post on dev.to

   If you have set the header of the post as `published: false`, change this value to `true`. Alternatively, if you you have edited the post in one sitting, hit **Save Changes** and your post will be published on dev.to.
