---
nav_order: 7
layout: page
permalink: /yaml
---

# YAML Basics

[YAML](https://yaml.org/){:target="_blank"} (YAML Ain't Markup Language) is a data serialization (fancy way of saying formatting data for the purpose of storage or transmission) language that is often used to create configuration files. Jekyll uses a combination of YAML and Liquid to separate data elements from formatting elements.

YAML is designed to be human-readable. It does not use any kind of angle brackets that are commonly used as markup tags. Instead, it uses blank spaces to form structures. Because of this, YAML is very particular about the placement of spaces. An extra space somewhere can easily make your file invalid. 

Each new level of data (aside from the firs) starts with an indent of **two spaces**. Each level also provides an access point to the data that you can reach using the dot notation (i.e. `site.data.dessert.icecream.flavor` would give you access to a folder named `_data`, in a file called `dessert.yml`, under _iceream_ data structure, a property named _flavor_.)

_Note: Because "tab" is not implemented the same way across editors, it's best to just type two spaces. With that said, it GitHub "tab" equates two spaces._

Two most common types of elements in YAML are mappings and lists. 
- Mapping is a simple key-value pair:

  ```
  key: value
  ```
  for example:
  
  ```
  flavor: chocolate
  ```
- A list is a sequence of items. Each item starts with a hyphen. For example:
 
  ```
  cells:
    - name: monocyte
    - name: macrophage
    - name: neutrophil
  ```
  
  You can use "for" loop to iterate through a list.
  
## YAML in Jekyll
  
In Jeykll, YAML is seen mostly at two locations: `_config.yml` file and the front matter of any page. 

### Front Matter

Front matter must be the first thing in the file and must take form of valid YAML set between triple dashed lines. Front matter tells Jekyll how to process and build your pages, creat and define define page-specific variables and trigger relevant file processings. Within front matter, you can set predefined variables or create your own. These variables will then be available through [Liquid](https://jekyllrb.com/docs/liquid/){:target="_blank"} tags within the same file or in any layouts or includes the current page/post relies on. 

A simple example of front matter would be:
```
---
layout: page
title: example of front matter
permalink: example
published: true
---
```
