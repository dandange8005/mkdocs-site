
## Why the project?

In DigEd team, we often required to create documentations or guides for different purposes. In a recent project, we were tasked to create an online resource to help staff to move over to Blackboard Ultra courses. We ended up creating the resource in Xerte which is a resource development tool for educators.

## Why Xerte
It was okay to use Xerte but there are some limitations:

- Xerte is not easy to collaborate with other team members
- There is no version control
- The search function is not great

## Why NOT Xerte

Though Xerte is a great tool for creating online resources, it is not ideal for creating documentations. Xerte doesn't come with a lot of features that are essential for creating documentations. 

For example, Xerte doesn't support Markdown syntax, it doesn't support version control, it doesn't support collaboration, it doesn't support search, etc.

- Xerte doesn't support Markdown syntax
- Xerte doesn't support version control
- Xerte doesn't support collaboration in a way that is easy to know who is working on what
- Xerte doesn't support search
- Xerte doesn't support localisation nativly
- Xerte Bootstrap template doesn't support multi-level navigation



## Github + MKDocs + Material for MKDocs

Idealy, we'd like to create a documentation/knowledge base site that is easy to maintain, easy to update, easy to collaborate, and easy to publish.

Below are some of the benefits of creating a project like this:

- Write the documentation in simply [Markdown](https://www.markdownguide.org/basic-syntax/) syntax (let you focus on writing the content not the style)
- Create a beatiful documentation site built with [MKDocs](https://www.mkdocs.org/) and [Material for MKDocs](https://squidfunk.github.io/mkdocs-material/)
- running a local server to test, preview the docs
- Github integration
  - version control
  - collaboration
  - track issues
  - [Github Codespace](https://github.com/features/codespaces)
  - doc deployed to Github pages and rendered with mkdocs + material for mkdocs theme
  - changes made locally or remotely all get published to the Github pages
- lots of great features from Material for MKDocs


### Github
I haven't started learning to use Git and GitHub until very recently. Here are some of the notes I took when I was learning Git and GitHub.

There are many benefits of using GitHub to host my notes and here are some of them:

- I don't need to worry about the losing of my notes as they are not just saved on my local computer, they are synched with the GitHub repo.
- I take advantages of GitHub to versioning my notes.
- I am able to work on my notes on multiple computers.
- I can collaborate with others on the same notes.
- I can publish my notes to the public.
- I can use GitHub to host my notes for free.


### MKDocs

MKDocs is a site generator for producing documentations. It is a static site generator that takes Markdown files and builds a static site out of them. It is a Python-based tool that is easy to install and use.

https://mkdocs.readthedocs.io/en/0.15.3/

### Material for MKDocs

MKDdocs is a site generator for producing documentations. Material on the other hand makes it looks good.

### Plugins for MKDocs + Material for MKDocs

[best-of-mkdocs](https://github.com/mkdocs/best-of-mkdocs) - A ranked list of awesome MkDocs projects and plugins.

- [mkdocs-static-i18n](https://github.com/ultrabug/mkdocs-static-i18n)
- [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin)
- [MkDocs Roamlinks Plugin](https://github.com/Jackiexiao/mkdocs-roamlinks-plugin)
- [MkDocs Awesome Pages Plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin)
- [mkdocs-callouts](https://pypi.org/project/mkdocs-callouts/)
- [mkdocs-video](https://github.com/soulless-viewer/mkdocs-video)
- mkdocs-git-authors-plugin
- mkdocs-git-committers-plugin
- mkdocs-toctree-plugin
- MkDocs PDF Export Plugin

## Tutorial

The tutorial I followed is this [How To Create STUNNING Code Documentation With MkDocs Material Theme](https://www.youtube.com/watch?v=Q-YA_dA8C20&list=WL&index=17&ab_channel=JamesWillett). 

<iframe width="560" height="315" src="https://www.youtube.com/embed/Q-YA_dA8C20" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Project layout

    .github/workflows/ # Github actions
      ci.yml
    mkdocs.yml    # The configuration file.
    docs/
      assets/ # Images and other files that are used in the docs
      index.md  # The documentation homepage.
      Getting Started/  # document folders, can be used for navigation
          doc 1.md
          doc 2.md
          doc 3.md
          doc 4.md
      stylesheets/ # Extra styles that can be added to the project


## prerequisites for the project
- python
- VS code
- Github Desktop (optional)
- some knowledge of Markdown syntax

## Setup workflow

Here are the steps to setup the project

1. Create you own repo on Github

    You can fork this repo or create your own repo on Github

2. Clone the repo to your local machine

    You can use Github desktop to clone the repo to your local machine

    Or you can use the command line to clone the repo

    ```bash
    git clone ...
    ```

3. install python

    You will need to install python to run the mkdocs server locally

    ```bash
    brew install python
    ```

4. create a virtual environment

    This step would allow you to install the python libraries locally without affecting the global python installation
   
    ```bash
    python -m venv venv
    ```

5. active the virtual environment

    You will need to activate the virtual environment before installing the python libraries.

    For Mac
    ```bash
    source venv/bin/activate
    ```

    For Windows
    ```git bash
    source venv/Scripts/activate
    ```

6. install mkdocs-material

    Install the mkdocs-material library

    ```bash
    pip install mkdocs-material
    ```
7. install the plugins

    ```bash
    pip install mkdocs-git-revision-date-localized-plugin
    ...
    ```
