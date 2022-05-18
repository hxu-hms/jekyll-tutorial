---
nav_order: 7
layout: page
title: YAML
parent: Jekyll Formatting Basics
---

# YAML

[YAML](https://yaml.org/){:target="_blank"} (YAML Ain't Markup Language) is a data serialization language (a fancy way of saying that YAML formats data for storage or transmission) that is often used to create configuration files. Jekyll uses a combination of YAML and Liquid to separate data elements from formatting elements.

## Basic formatting
YAML is designed to be human-readable. It does not use any kind of angle brackets that are commonly used as markup tags. Instead, it uses blank spaces to form structures. Because of this, **YAML is very particular about the placement of spaces.** An extra space somewhere can easily make your file invalid. 

Two most common types of elements in YAML are mappings and lists. You will see both of these in a Jeykll site.
 
- Mapping is a simple key-value pair:

  ```
  key: value
  ```
  for example:
  
  ```
  flavor: chocolate
  ```
- A list is a sequence of items. Each item starts with two spaces (or a tab in some editors) of indent and a hyphen. For example:
 
  ```
  cells:
    - name: monocyte
    - name: macrophage
    - name: neutrophil
  ```

_Note: Because "tab" is not implemented the same way across editors, it's best to just type two spaces. With that said, in GitHub "tab" equates two spaces._

## YAML in Jekyll websites
  
In Jeykll, YAML is seen mostly within  `_config.yml` file and the "front matter" of any page (including the homepage banner). 

### Homepage banner
YAML formatting is used for the website homepage banner - be sure to follow the [Basic formatting](./yaml#basic-formatting) suggestions shown below when editing the banner text and links.

### Front Matter

**Front matter** tells Jekyll how to process and build your pages, create & define page-specific variables, and trigger relevant file processings.

- Front matter must be the first thing in the file
- Front matter must take form of valid YAML set between triple dashed lines. 
- Within front matter, you can set predefined variables or create your own.
	- These variables will then be available through [Liquid](https://jekyllrb.com/docs/liquid/){:target="_blank"} tags within the same file or in any layouts or includes the current page/post relies on. 

An example of front matter would be:
```
---
layout: page
title: Example # will display as the page name on the left navigation bar
permalink: example # defines page URL
published: true
nav_exclude: false # toggle to true to exclude this page from naviation bar
has_children: false # toggle to true if this page has subpages
parent: Motivation # defines this page as a subpage of the page titled "Motivation"
---
```

**Read more about controlling page navigation structure on your site in [Just the Docs](https://labsyspharm.github.io/just-the-docs-lsp/docs/navigation-structure/){:target="_blank"} .**

  
