---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
permalink: /
is_menu_entry: true
position: left
order: 1
layout: page
title: Home
---
# Development presentations
This Github project aim contains the developpers presentations. 

## Technologies
The presentations are written in [Markdown](https://www.markdownguide.org/cheat-sheet/){:target="_blank"} and use [Github pages](https://pages.github.com/){:target="_blank"}, [Github actions](https://docs.github.com/fr/actions){:target="_blank"} and [Marp](https://marp.app/){:target="_blank"}.

## New presentations
The new presentations should be created under the directory docs.<br/>
A TOC can be generated in a presentation by inserting the comments:
```
<!--ts-->
<!--te-->
```
The title for level 1 an 2 will be used to generate the table of content via the utilitary 
[github-markdown-toc ](https://github.com/ekalinin/github-markdown-toc){:target="_blank"} (gh-md-toc).
gh-md-toc is executed vi the Github actions, step Toc generation. If the file does not contain the comments for the toc it is ignored (this an be traced in the github actions outputs).

![Presentation toc generation](./img/gh-actions-toc-step.png)
*Toc generation output in Github actions*

## Presentations list.
A main TOC (a presentations list) is generated an inserted in the index file via the Github actions. It uses the script [generate-toc.sh](https://github.com/avenirs-esr/presentations/blob/c78d67f3ce3eaa1c33e7458a8cb6a57f60d84f6a/scripts/generate-toc.sh){:target="_blank"}. 

The insertion slot is determined by the comment
`<!-- {{TOC}} -->` in the file index.template.md.
