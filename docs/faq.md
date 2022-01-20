---
layout: default
title: FAQs
nav_order: 8
permalink: /faq
---
# Frequently Asked Questions

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## How do I change the font size of the whole website?

If you want to alter the default font size globally, [documentation](https://labsyspharm.github.io/just-the-docs-lsp/docs/utilities/typography/#global-font-size-adjustments) for the LSP/HiTS theme provides details instructions. 

[View Documentation Here](https://labsyspharm.github.io/just-the-docs-lsp/docs/utilities/typography/#global-font-size-adjustments){: .btn .btn-arrow }

Briefly, here are the steps:

1. Make a new color scheme file (with the extention `.scss`) under `docs/_sass/color_schemes/`
2. Copy and paste the content of your chosen color scheme from the theme repository into your new color scheme file - this will tell the theme to keep using the same colors and other settings
3. In your new color scheme file, override the font sizes with lines like these:

```
$body-font-size: fs-3;
$h2-font-size: fs-8;
# h2 refers to the level 2 heading
```
4. Call your new color scheme file in `_config.yml`
```
color_scheme: NEW_SCHEME_FILE_NAME
```

## How do I change the size of an embedded image?

There are a few ways to insert an image and scale its size. Not all the Markdown solutions I've come across online are supported by GitHub Pages. One method that works is to use a little HTML instead of Markdown.

```
<img src="drawing.jpg" alt="drawing" width="200"/> 
```
or
```
<img src=http://...jpg width=“200” height=“200” />
```

Note that `alt=` is setting the alternative text for the image, when the image cannot be viewed for any reason. 

As an example, here's the same image inserted at the orginal size and then scaled smaller:
```
![original size neuron drawing](./images/neuron-drawing.jpg)
<img scr='images/neuron-drawing.jpg" alt="smaller neuron drawing" width="300"/>
```

![original size neuron drawing](./images/neuron-drawing.jpg)  

## How do I exclude a page from showing up in navigation?
          
You may want to exclude some pages from navigation and only lead viewers to them via links. To accomplish this, you can choose from two expressions in the front matter of that page:
```
---
exclude: true
---
```
or
```
---
nav_exlude: true
---
```

## How do I create a link that opens a new tab by default?

You can use the following addition to the link syntax:
```
[new tab link](https://mcmicro.org/){:target="_blank"}
```
It should render: [new tab link](https://mcmicro.org/){:target="_blank"}


          
