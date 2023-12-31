# MKDocs

MKDocs is a site generator for producing documentations. It is a static site generator that takes Markdown files and builds a static site out of them. It is a Python-based tool that is easy to install and use.

You can find the official documentation for MKDocs here: https://mkdocs.readthedocs.io/en/0.15.3/

## Why MKDocs

MKDocs is a great tool for creating documentations. It is easy to install and use. It is also easy to collaborate with other team members. It supports Markdown syntax, version control, collaboration, search, etc.

## Material for MKDocs

Material for MKDocs is a theme for MKDocs.

You can find the official documentation for Material for MKDocs here: https://squidfunk.github.io/mkdocs-material/

## Plugins for MKDocs + Material for MKDocs

There are many plugins for MKDocs and Material for MKDocs. Here are some of them:

- [best-of-mkdocs](https://github.com/mkdocs/best-of-mkdocs) - A ranked list of awesome MkDocs projects and plugins.
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

## Setting up MKDocs

There are many ways to install MKDocs. I followed this [tutorial](https://www.youtube.com/watch?v=Q-YA_dA8C20&list=WL&index=17&ab_channel=JamesWillett) to install MKDocs and Material for MKDocs.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Q-YA_dA8C20" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### Pre-requisites

- Python
- VS Code

### Step by step process
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

    - Go to the project folder
    - Open the terminal
    - Activate the virtual environment

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
8. run the mkdocs server

    ```bash
    mkdocs serve
    ```

### Basic project structure

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
