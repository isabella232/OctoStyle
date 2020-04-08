---
layout: page
title: Working with images
order: 40
permalink: images
family: language
---

## Screenshots 

When you're demonstrating how to complete a task in a UI, screenshots can be incredibly useful. When used well, they reassure users they’re on the right path and make following the steps a frictionless process. However, it is important not to over-rely on screenshots as UIs change and users can be left confused when the screenshot doesn't match the UI.

To help get the balance right, think of screenshots as signposts along the way. Don’t include screenshots for every step of a procedure, but to orient the user if:

- They might struggle to locate an item in the UI.
- The procedure jumps from one place in the UI to another.
- You want to reassure them they’re in the right place.
- For accessibility reasons, it’s also important not to rely solely on screenshots to convey information to users. When including screenshots, please also describe the actions you expect the user to take.

Make sure any information that is conveyed in the screenshot is done so to supplement the text. If the UI changes and important steps are only documented with images, the user might not be able to follow the instructions.

## Rules for screenshots

1. Don't include the browser window

    When you take screenshots of web pages, don't include the browser window "chrome" - the stuff around the page. Just include the page itself.

1. Don't include version warning bars

    Alpha and beta builds include the orange warning bar. Don't include it in screenshots.

1. Sample data should look realistic

    Take time to set up data that looks and feels somewhat realistic. Don't use your name. 

1. Include enough of the window to orient users

	Typically, in the Octopus Web Portal include the navigation bar at the top of the page and the content of the screen you want to share.

1. Don't stack screenshots

    If want to include a screenshot that extends past the viewable window, use a tool like Snagit to capture a scrolling screenshot.

1. Reduce the whitespace

    Don't take screenshots that are too wide, or include too much content at the bottom. Set your browser to somewhere between 1200px and 1400px wide.

1. Don't include the help window

	The help text is incredibly useful in the Octopus Web Portal, but it will make screenshots look crowded.

1. Use green call-outs

	Use green call-outs when you need to draw attention to some aspect of the UI. 

	Use these colors:
	1. RGBA: 0, 204, 101, 255
	1. Hex: 00CC65

1. Don't include the mouse cursor

1. Don't use screenshots to show commands the user needs

    If the commands are in a screenshot, the user must manually copy them. Add them to a code block instead.

1. Include app windows

    When you take a screen of an app, for instance, Tentacle Manager, include the full window so users don't think they're seeing a webpage.

1. Don't take screenshots over Remote Desktop
	
	Remote desktop tunes down colors and disables clear type, so fonts look rubbish.

## The Octopus Web Portal

The Octopus UI has a light theme and a dark theme. We want our readers to have a consistent experience across our site when they see images of the UI. Unless you are specifically discussing the dark mode theme, use light mode for screenshots of the Octopus Web Portal.

## Related pages

See [adding images with markdown]({{site.url}}/{{site.baseurl}}/markdown#images).
