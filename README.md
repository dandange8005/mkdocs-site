# Introduction

This is my experimental github repository that uses Github and mkdocs + Material theme to publish my notes. 

The notes are published at https://dandange8005.github.io/mkdocs-test/ using Github pages.

The tutorial I followed is this [How To Create STUNNING Code Documentation With MkDocs Material Theme](https://www.youtube.com/watch?v=Q-YA_dA8C20&list=WL&index=17&ab_channel=JamesWillett). 

## Why create a project like this?

In our DigEd team, we are often required to create documentations or guides for different purposes. In a recent project, we were tasked to create an online resource to help staff to move over to Blackboard Ultra courses. We ended up created the resource in Xerte which is a resource development tool for educators.

It was okay to use Xerte but there are some limitations:

- Xerte is not easy to collaborate with other team members
- There is no version control
- The search function is not great

We wanted to create a documentation site that is easy to maintain, easy to update, easy to collaborate, and easy to publish.

Below are some of the benefits of creating a project like this:

- Write the documentation in simply [Markdown](https://www.markdownguide.org/basic-syntax/) syntax (let you focus on writing the content not the style)
- Create a beatiful documentation site built with [MKDocs](mkdocs.org) and [Material for MKDocs](https://squidfunk.github.io/mkdocs-material/)
- running a local server to test, preview the docs
- Github integration
  - version control
  - collaboration
  - track issues
  - [Github Codespace](https://github.com/features/codespaces)
  - doc deployed to Github pages and rendered with mkdocs + material for mkdocs theme
  - changes made locally or remotely all get published to the Github pages
- lots of great features from Material for MKDocs

## prerequisites for the project

- python
- Github CLI
- VS code
- Github Desktop (optional)
- some knowledge of Markdown syntax

## Setup workflow

Here are the steps to setup the project

```bash
python -m ven venv
source venv/bin/activate
```


## Editing the Docs

### Editors

You can choose whatever editor you want to make changes to the .md files as they use Markdown syntax.

However, these are some of the editors I would consider using

- VS code (with markdown preview)
- Obsidian

### Editing on the original local machine

The original machine will include the python library which will not be synched to Github as they will be added to the .gitignore file

#### Steps to make changes

run vs code
editing in vs code
commit the changes

### Editing remotely

There are a few options you can choose to edit the documents remotely

#### Run codespace via Github

- This would allow you to make changes to the repo and the docs within the browser

#### Clone the repo to your local machine

- Github desktop

- open up the repo with either obsidian, Marktext or VS code


## Material for MKDocs

### plugins used in the project

- search
- [roamlinks](https://github.com/Jackiexiao/mkdocs-roamlinks-plugin)
- [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin)
- [mkdocs-i18n](https://gitlab.com/mkdocs-i18n/mkdocs-i18n)
- [mkdocs i18n](https://github.com/ultrabug/mkdocs-static-i18n)] 
- [Best of mkdocs](https://github.com/mkdocs/best-of-mkdocs)
