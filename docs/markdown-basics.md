---
layout: page
nav_order: 3
permalink: markdown-basic
---

# Markdown Basic Syntax

This page will give you a quick guide through some of the Markdown syntax that you may use to edit your `.md` files. If you are editing in GitHub, the Preview button on top of the editing window allows you to view basic Markdown contents before you commit to the changes (Jekyll-specific features are not supported).

## Headings

Adding number sign `#` followed by a space in front of a line creates a heading. The number of `#` added corresponds to heading level.  
Leave a blank line before and after the heading for best practice. 

| Markdown | Rendered Output |
|----------|-----------------|
| `# Heading 1`| <h1> Heading 1 </h1> |
|`## Heading 2`| <h2> Heading 2 </h2> |
|`### Heading 3`| <h3> Heading 3 </h3> |

## Paragraph breaks

To break between paragraphs, use a blank line to seprate the paragraphs.

| Markdown | Rendered Output |
|----------|-----------------|
| <p>`This is the first paragraph.`</p> <p>`This is the second paragraph.`</p>| <p>This is the first paragraph.</p> <p>This is the second paragraph.</p> |

## Line breaks

To create a line break, end a line with two or more spaces, then type return.

| Markdown | Rendered Output |
|----------|-----------------|
|`This is the first line.   `<br> `This is the second line.`|This is the first line.<br> This is the second line.|

## Bold

Use two asterisks before and after a word of phrase to make it **bold**.

| Markdown | Rendered Output |
|----------|-----------------|
|`This is **bold**`|This is **bold**|

## Italic

Use one asterisk before and after a word or phrase to italicize it. 

| Markdown | Rendered Output |
|----------|-----------------|
|`This is *italic*`|This is *italic*|

## Lists

### Ordered lists

Use number followed by a period and a space for line items in an ordered list. When editing in GitHub, numbers will autofill in numeric order. When editing locally, numbers don't have to follow numeric order, but lists should start at number 1.  

| Markdown | Rendered Output |
|----------|-----------------|
|`1. item`<br>`2. item`<br>`3. item`|<ol><li>item</li> <li>item</li> <li>item</li></ol>|

When editing in GitHub, add two `tab` to start a nested list. For example,

```
1. one
2. two
   1. sub-one
   2. sub-two
```

will render

1. one
2. two
    1. sub-one
    2. sub-two

## Unordered lists

Use dash `-`, asterisk `*`, or plus sign `+` followed by space in front of an item in an unordered list. When editing in GitHub, GitHub will autofill the sign after the first item is entered.

| Markdown | Rendered Output |
|----------|-----------------|
|`- one`<br> `- two`<br> `- three`|<ul><li>one</li> <li>two</li> <li>three</li></ul>|

Use one `tab` to create a nested unordered list on GitHub. For example

```
- one
- two
  - sub-one
  - sub-two
```

will render

- one
- two
  - sub-one
  - sub-two

## Codes

Use backtick ` to enclose codes. Use ``` to enclose blocks of code.

| Markdown | Rendered Output |
|----------|-----------------|
|`` `code` ``| `code`|

And for example

`` ``` `` <br>
```a block of code ```<br>
```all code ``` <br>
`` ``` ``

would render

```
a block of code
all code
```

To show backticks `` ` `` in code, surround the portion of code that would include backticks in double backticks. (Yes, this is confusing. Use Preview a lot to check your work here)

| Markdown | Rendered Output |
|----------|-----------------|
|``` `` ` `` ```| `` ` ``|

## Links

### Absolute links

### Relative links

## Images



