+++
title = "Article Settings"
description = "Customizations for posts."
weight = 103
template = "page.html"
+++

<img src="../../assets/screenshots/article-right-click.png" alt="Article Right Click" class="screenshot" />

To customize a post, simply right-click on the post and choose "Settings." This will display a panel offering a range of customization options.

<img src="../../assets/screenshots/article-settings.png" alt="Article Settings" class="screenshot" />

## Slug

By default, each post URL uses its UUID, like this:

<a href="https://planetable.eth.limo/77BB1A2A-971C-443B-A1F4-F50F205525EF/" target="_blank">https://planetable.eth.limo/77BB1A2A-971C-443B-A1F4-F50F205525EF/</a>

You can enter a custom slug here to change the URL to something like:

<a href="https://planetable.eth.limo/introducing-planet/" target="_blank">https://planetable.eth.limo/introducing-planet/</a>

Only lowercase letters, numbers, and hyphens can be used in the slug.

## Type

By default, each post has a "blog" type, meaning it will appear chronologically on the homepage and be included in the RSS feed. However, for pages like "About Us," you may not want them to appear as blog posts on the homepage. In this case, you can select the "Page" type here.

## Navigation

If `Include in Site Navigation` is checked, the post will be included in the site-level navigation. For example, if you have an "About Us" page and want to display it at the top level, this is the option for you.

`Navigation Weight` is an integer used for ordering; smaller numbers appear first.

## External Link

If you want an item in the site-level navigation to redirect to another URL, you can enter that URL here.