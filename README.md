This is my experimental github repository that uses Github and mkdocs + Material theme to publish my notes. 

The notes are published at https://dandange8005.github.io/mkdocs-test/ using Github pages.

The tutorial I followed is this [How To Create STUNNING Code Documentation With MkDocs Material Theme](https://www.youtube.com/watch?v=Q-YA_dA8C20&list=WL&index=17&ab_channel=JamesWillett). 

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

1. create you own repo on Github
2. clone the repo to your local machine
3. install python
4. create a virtual environment
   
    ```bash
    python -m venv venv
    ```

5. active the virtual environment

    ```bash
    source venv/bin/activate
    ```

6. install mkdocs-material

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
- [mkdocs-static-i18n](https://github.com/ultrabug/mkdocs-static-i18n)
- [Best of mkdocs](https://github.com/mkdocs/best-of-mkdocs)
