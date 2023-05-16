# Pandoc

## Overview

GitHub: [pandoc](https://github.com/jgm/pandoc)

Pandoc is a Haskell library for converting from one markup format to another, and a command-line tool that uses this library.

## Installation

I've installed Pandoc on my Macbook Pro using Homebrew on 04.05.2023

```bash

MacOS: `brew install pandoc`

```bash
$ pandoc --version
```

## Examples

### Convert Word to Markdown

```bash
$ pandoc -f docx -t markdown -o pandoc.md pandoc.docx
```


### Convert Markdown to HTML

```bash
$ pandoc -f markdown -t html5 -o pandoc.html pandoc.md
```

## Links
[How to Easily Convert Word to Markdown with Pandoc](https://medium.com/geekculture/how-to-easily-convert-word-to-markdown-with-pandoc-4d60878ccc64)
