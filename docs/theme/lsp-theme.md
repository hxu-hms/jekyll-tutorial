---
layout: page
title: LSP Custom Theme
permalink: lsp-theme/
nav_order: 4
has_children: true
---
# LSP Custom Theme

This section is a guide on the LSP theme: how to apply the theme, LSP/HiTS-related theme elements and several styling components that may be most relevant for showcasing your research.

However, this is not a complete documentation. For information on the rest of the theme, you can check out the [documentation](https://labsyspharm.github.io/just-the-docs-lsp/){:target="_blank"} and [repository](https://github.com/labsyspharm/just-the-docs-lsp){:target="_blank"}.

# Applying the Theme

If you are starting with the website templates, the LSP theme is already applied to the template. 

{: .fs-5 }
{: .fw-300 }
Proceed to [Customizations](./lsp-customizations.md) to adjust styling elements to your liking.

---

If you are starting a website from scratch, or adapting your existing Jekyll website to use the LSP theme. Follow these steps:

1. In `_config.yml` file, insert the following line (to replace the esiting `theme` or `remote_theme` variable)
    ```
    remote_theme: labsyspharm/just-the-docs-lsp
    ```

2. Make sure that remote theme is enables by adding
    ```
    plugins:
        - jekyll-remote-theme
    ```





