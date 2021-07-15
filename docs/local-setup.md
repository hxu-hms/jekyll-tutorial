---
layout: page
title: Setting up a Jekyll Website Locally
permalink: local-setup
parent: Quick Start
nav_order: 2
---
# Before the Start
The following step-by-step guide will help you create a Jekyll site to be hosted on GitHub. Before we start, here are some helpful notations to know:
```
$ denotes the start of a command line. You type these command lines into your command prompt window and press Enter to execute it.
# denotes a note or description. You do not need to type this.
```

# Installing Jekyll
Jekyll documentation provides step-by-step guides for installation on macOS, Windows, Ubuntu and other Linux systems. 

Please head to [Installation](https://jekyllrb.com/docs/installation/#requirements) on Jekyll documentation to choose your OS and follow along.

# Setting up a Website (To be hosted on GitHub)

1. Create a new repository on Github to store your site's source code. If you already have an existing repository, you can store the source code in a `/docs` folder

2. Make sure to set visibility of your repository to __public__, in order to have your website hosted on GitHub.

3. If you don't already have a local copy of your repository _(if you do, jump to step 7)_,  navigate to a location on your computer where you would like to store your website's source files. In your terminal, replace `PARENT-FOLDER` with the folder of your choosing.
    ```
    $ cd PARENT-FOLDER
    # changes directory to PARENT-FOLDER
    # Note that if you are working on a Linux subsystem, you may need a /mnt/ prefix to your path
    ```
4. Initialize a local Git repository in the `PARENT-FOLDER`, using the name of your repository instead of `REPOSITORY-NAME`. 
    ```
    $ git init REPOSITORY-NAME
    ```
5. chnage directories to the repository.
    ```
    $ cd REPOSITORY-NAME
    ```
6. Navigate to the publishing source of your website. For example if you chose to store files of your webiste in `docs` folder, create and change directories to `docs` folder.
    ```
    $ mkdir docs
    # Creates a new folder called docs
    $ cd docs
    ```
    If you chose to publish your site from a branch other than the `main` (for example, `gh-pages` is recommended), you can create and check out that branch.
    ```
    $ git checkout --orphan gh-pages
    # Creates a brand new branch called gh-pages and switches to gh-pages branch
    ```

7. Now that you are on the directory and branch of your chosen publishing source, create a new Jekyll site with `jekyll new` command.
    ```
    $ jekyll new .
    # Creates your site in the current directory
    ```
    Following this command, Jekyll gets to work and creates a sleu of files for your website. These include two folders:
    ```
    _posts
        # where future posts on your website can be stored

    _site
        # where the finished product of your website is stored. These are automatically updated as you edit the files of your site.
    ```
    And several files:
    ```
    .gitignore
    _config.yml
        # Jekyll uses information in here to configure the website
    404.html
    about.md
        # this is a page with some default content that will appear on your site (unless overwritten)
    Gemfile
        # contains a list of Ruby gems used by your site
    Gemfile.lock
    index.md
        # this is an empty home page that is created by default
    ```
8. Open `Gemfile` Jekyll created, add `#` to the beginning of the line `gem "jekyll"` to comment it out. 
9. Edit the line starting with `# gem "github-pages"` to the following:
    ```
    gem "github-pages", "~> GITHUB-PAGES-VERSION", group :jekyll_plugins
    ```
    Replace `GITHUG-PAGES-VERSION` with the lates supported version of the `github-pages` gem, which you can find on the [Dependency versions](https://pages.github.com/versions/) page.
10. Save and close the `Gemfile`.
11. From command line, run `bundle update`.

# Testing Site Locally
At this stage you can already preview and test your blank site on your local server. It is highly recommended that you test your site multiple times locally, throughout the building process. 
1. To do so, run 
    ```
    $ bundle exec jekyll serve
    ```
    Output on your command line will indicate `Server running... press ctrl-c to stop.` at the end, when running correctly.
2. To preview the site, in your web browser, navigate to `http://localhost:4000`.

_Ta-dah! Your website!_

# Commit your work and set up GitHub Pages
