# Introduction

This is a test repository using mkdocs + Material Template. 

You can visit the published test site at: https://dandange8005.github.io/mkdocs-test/

## Tutorial I followed

I followed this tutorial ([How To Create STUNNING Code Documentation With MkDocs Material Theme](https://www.youtube.com/watch?v=Q-YA_dA8C20&list=WL&index=17&ab_channel=JamesWillett)) to create this project. 

## Why create a project like this?

In our DigEd team, we are often asked to create documentations for different proejcts. In a recent project, we were asked to create an asynchronous online resource for Blackboard Ultra courses. The resource will be used by staff to learn how to use Blackboard Ultra. We created the resource using Xerte Online Toolkits.

It was okay to create online learning resources using Xerte but it was not ideal for creating documentations. We wanted to create a documentation site that is easy to maintain, easy to update, easy to collaborate, and easy to publish.

Below are some of the benefits of creating a project like this:

- Write the documentation in simply [Markdown](https://www.markdownguide.org/basic-syntax/) syntax (let you focus on writing the content not the style)

- Create a beatiful documentation site built with [MKDocs](mkdocs.org) and [Material for MKDocs](https://squidfunk.github.io/mkdocs-material/)

- running a local server to test, preview the docs

- Github integration
  
  - version control
  
  - collaboration
  
  - track issues
  
  - [Github Codespace](https://github.com/features/codespaces)
  
  - doc deployed to Github pages and rendered with mkdocs + material for mkdocs
  
  - changes made locally or remotely all get published

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
- [Marktext](https://github.com/marktext/marktext)
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
