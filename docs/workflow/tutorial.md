---
layout: page
title: Tutorial
permalink: /tutorial
nav_order: 3
has_children: true
---
# Tutorial

1. If you don't have one yet, [sign up](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) for a GitHub personal account. 

    Contact Jeremy Muhlich (Jeremy_Muhlich@hms.harvard.edu) to join the GitHub organization **Laboratory of Systems Pharmacology @ Harvard** (labsyspharm)

    <br>

2. Start a new repository under [**Laboratory of Systems Pharmacology @ Harvard**](https://github.com/labsyspharm){:target="_blank"}. Choose _Import a repository_, on the right side of the title. For more information on the Import function, you can check out GitHub's [Documentation](https://docs.github.com/en/github/importing-your-projects-to-github/importing-source-code-to-github/importing-a-repository-with-github-importer){:target="_blank"} on it.

    <br>

2. Use the URL for the blank site template `https://github.com/labsyspharm/blank-method-microsite/` or `https://github.com/labsyspharm/blank-software-website` as _old repository's clone URL_ and set **labsyspharm** as the owner.

    <img src="images/import-screenshot.PNG" alt="import_example" width="600"/>


    <br>

    {: .fs-3 }
    {: .fw-300 }
    Note: Learn more about the LSP-themed templates available to you on the [Website Templates](../website-template.md) page.

    <br>

3. Edit the template. You can either edit on GitHub or work with Jekyll locally. 

    *Both options involvings writing your content using Markdown and YAML. Checkout the [Jekyll Formatting Basics](../formatting-basics.md) to get you started.*

    <br>

    {: .fs-5 }
    {: .fw-500 }
    Option 1: Edit on GitHub

    i. Use the edit function (pencil icon) on GitHub to [edit](./import-template.md#editing-pages-on-github) pages on GitHub

    ii. [Add](./import-template.md#adding-pages-on-github) new pages for additional content when needed

    <br>

    {: .fs-5 }
    {: .fw-500 }
    Option 2: Use Jekyll locally

    i. [Install](./local-setup.md#installing-jekyll) Jekyll following documentation

    ii. [Clone](./local-setup.md#starting-a-local-website-repository) your website repository to your local computer

    iii. [Test](./local-setup.md#testing-site-locally) your site locally

    iv. [Apply](./local-setup.md#commiting-your-work) your changes to the repository

    <br>

4. Set up GitHub Pages to make your website public

    i. Make sure your repository access is set to **public**. This can be changed under **Settings > Manage access**.

    ii. Within Settings, head over to **Pages** and change the default Source to the branch and folder where your website files are stored.

    iii. Click "Save" after configruing the source. A banner should show up to show that your website is "Your site is ready to be published at *url*" and eventually "your site is published at *url*" (This process might take a few minutes).

    ![screenshot of banner](../images/ghpages-setup.jpg)

    Now, if you head to the displayed *url*, you should see your finished website. 

    <br>

{: .fs-5 }
{: .fw-500 }
**Now you have a website that you can preview and edit. [LSP Custom Theme](../theme/lsp-theme.md) page will guide you through the first steps of cutomizing your website.**