---
layout: page
title: LSP Custom Theme
permalink: lsp-theme/
nav_order: 5
---
# LSP Custom Theme
{: .no_toc }

This page shows elements from the LSP theme along with instructions on how to customize them for your website. These are elements that may be most relevant to an academic website design. 

However, this is not an all-emcopassing list. For information on the rest of the theme, you can check out the [documentation](https://jegra.github.io/just-the-docs/) and [repository](https://github.com/jegra/just-the-docs/) (LSP-specific theme is under `hms` branch).

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Applying the Theme

If you are importing the blank website template, the LSP theme is already applied to the template. You can add, edit or remove the elements based on your need.

If you are starting a website from scratch, or adapting your existing Jekyll website to use the LSP theme. You need to

1. In `_config.yml` file, insert the following line (to replace the esiting `theme` or `remote_theme` variable)
    ```
    remote_theme: jegra/just-the-docs@hms
    ```

2. Make sure that remote theme is enables by adding
    ```
    plugins:
        - jekyll-remote-theme
    ```

# Hero Banner

Hero banner and text shows off your content immediately on the home page. It looks something like this:

<div class="row">

<div class="col-xs-12 col-sm-12">
<div markdown="1">
![hero banner](../images/hero-banner.png)
</div>
</div>

</div><!-- end grid -->

To make a hero graphic banner:
1. Add your image of choice to the repo. We suggest adding it to a central folder where you keep all images for the site (e.g. `assets/images/`). 
2. In `_config/yml` file, use the following line to embed hero image. Replace `DIRECTORY` to the path to your chosen image
    ```
    hero_background: "DIRECTORY"
    ```
    e.g. `hero_background: "/assets/images/hero_background.jpg"`
3. In the front matter of your home page, define the following values
    ```
    # Hero heading and body text
    hero_heading: "THIS IS THE HEADING"
    hero_body: "This is the body text."

    # Call to action(CTA) buttons to be displayed within the hero area
    # 'label', 'link', and 'target' values can be specified for each
    hero_ctas:
    - label: "button 1"
        link: "#getting-started"
    - label: "button 2"
        link: "http://github.com/"
        target: "_blank"

    # 'target' attribute specifies where to open the link. '_blank' opens a new tab, '_self' opens the link in the same tab etc. Default is opening in the same tab.
    ```
For more information on hero banner, check out [theme documentation](https://jegra.github.io/just-the-docs/docs/ui-components/hero/).

# Header Logos

# Footer

## Footer logos

## Licenses

## Edit this Page on GitHub

## Last Modified Date

# Highlighted Stlying Elements and UIs

Stlying elements and UIs in this template is well-documented by the designer. This section will highlight a few elements and UIs that may be the most relevant for your website and point to their documentations.

## Basic Grid

The basic grid is an esay way to inject visual intrigue into your site's layout. It is also a great method of showing off parallel pieces of information. The results looks like this

![basic grid](../images/basic-grid.png)


## Enhanced Grid

## Image Cards

## Navigation

## Video Embedding




