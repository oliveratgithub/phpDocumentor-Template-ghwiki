# GitHub Wiki-Template for phpDocumentor

## Introduction
This is a custom template to use with [phpDocumentor](https://github.com/phpDocumentor/phpDocumentor).

It is intended to create the code documentation as markdown files, fully compatible to serve as a [GitHub Wiki](https://help.github.com/en/github/building-a-strong-community/about-wikis) in a GitHub repository of your choice.

### Example
You can find a live example in this repository's Wiki: [zorgch/zorg-code/wiki](https://github.com/zorgch/zorg-code/wiki)

## Installation and usage
### Pre-requisites
* [phpDocumentor](https://github.com/phpDocumentor/phpDocumentor/releases) must be installed or available using its `.phar`
* You have a GitHub Wiki [cloned locally](https://help.github.com/en/github/building-a-strong-community/adding-or-editing-wiki-pages#adding-or-editing-wiki-pages-locally)

### Generate GitHub Wiki Markdown from your code
1. Download & unpack - or clone - this repository to your computer
2. Specifiy this template `phpDocumentor-Template-ghwiki` while generating your code documentation using `phpDocumentor`:

`php ./phpDocumentor.phar -d "/path/to/my/sourcecode" -t "/path/to/local/github-wiki" --template="/path/to/phpDocumentor-Template-ghwiki" --cache-folder "/path/to/store/cache" --title "My code project"`
  * _NOTE_: you may get an error at the end of the parsing - which you can just ignore, all work was done:
  `ERROR In PathGenerator.php line 120: Variable substitution in path /namespaces/{{name}}.md failed, variable "name" did not return a value`
3. The target directory `/github-wiki` consists of various markdown (.md) files now
4. Review, commit & push your local GitHub Wiki repository changes
5. Browse to the Wiki on the corresponding GitHub repository to see your code documentation online
