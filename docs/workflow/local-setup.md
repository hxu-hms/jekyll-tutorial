---
layout: default
title: Working with Jekyll Locally
permalink: local-setup
parent: Tutorial
nav_exclude: false
nav_order: 4
---
# Before the Start
{: .no_toc }

{: .fw-300 }
Before we start, here are some helpful notations to know:
```
$ denotes the start of a command line. You type these command lines into your command prompt window and press Enter to execute it.
# denotes a note or description. You do not need to type this.
```
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Installing Jekyll
Jekyll documentation provides step-by-step guides for installation on macOS, Windows, Ubuntu and other Linux systems. 

Please head to [Installation](https://jekyllrb.com/docs/installation/#requirements){:target="_blank"} on Jekyll documentation to choose your OS and follow along.

# Starting a local website repository

{: .fw-300 }
GitHub's documentation describes in detail [how to start a Jekyll website *from scratch* locally](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll){:target="_blank"}. 

Here, we will only elaborate on how to use the blank templates locally. 

1. Follow the instructions to [import the templates](./import-template.md#importing-template-repository-on-github).

    Now you should have a repository with *your website name*. 

2. Clone your website repository
    - This will insert blank-method-microsite files into your current directory
    - You can find the https link for your new repo on the green 'code' button on the main repo page

    ```
    $ git clone <https>
    ```

3. Navigate to the `docs` folder in your local repository. From command line, run `bundle install`. This will install the necessary gems for your website
    ```
    $ cd your-website-name/docs
    $ bundle install
    ```

4. You are now all set to work on your site locally. You can add pages by making new `.md` files and edit them in your text editor of choice. 

# Testing site locally
You can already preview and test your site on your local server. It is highly recommended that you test your site multiple times locally, throughout the building process. 

1. To do so, while in the `docs` folder, run 
    ```
    $ bundle exec jekyll serve
    ```
    Output on your command line will indicate `Server running... press ctrl-c to stop.` at the end, when running correctly.

2. To preview the site, in your web browser, navigate to `http://localhost:4000`.

# Commiting your work

1. To make your edits final, you need to add and commit your changes (if these terms are foreign to you, check out this [Git Guide](https://github.com/git-guides/){:target="_blank"} for some background knowledge on the basic actions of Git)
    ```
    $ git add .   # adds all the changes in the current directory
    $ git commit -m 'Initial GitHub pages site with Jekyll'

    # Note that -m allows you to add a message to decribe your commits. Content in the quotes is an example.
    ```

2. Add your website repository on Github.com as a remote destination, replacing `USER` with the account name that owns the repository (`labsyspharm` in most cases), and `REPOSITORY` with the name of the repository
    ```
    $ git remote add origin https://github.com/USER/REPOSITORY.git
    ```
    If you started with cloning your repository, you may already have the remote origin set up. You can check with the command `git status`

3. Push the repository to GitHub, replacing `BRANCH` with the name of the branch you are working on. Now your repository is updated with the changes you made locally.
    ```
    $ git push -u origin BRANCH
    ```


{: .fs-5 }
{: .fw-300 }
>Go back to Tutorial page to finish setting up your website.
>[Back to Tutorial](./tutorial.md){: .btn .btn-outline .btn-arrow }
