
# Development presentations
This Github project aim contains the developpers presentations. 

## Technologies
The presentations are written in <a href="https://www.markdownguide.org/cheat-sheet/" target="_blank">Markdown</a> and use [Github pages](https://pages.github.com/){:target="_blank"}, [Github actions](https://docs.github.com/fr/actions){:target="_blank"} and [Marp](https://marp.app/){:target="_blank"}.

## New presentations
The new presentations should be created under the directory docs.<br/>
A TOC can be generated in a presentation by inserting the comments:
```
<!--ts-->
<!--te-->
```
The title for level 1 an 2 will be used to generate the table of content via the utilitary 
[github-markdown-toc](https://github.com/ekalinin/github-markdown-toc){:target="_blank"}.
gh-md-toc is executed vi the Github actions, step Toc generation. If the file does not contain the comments for the toc it is ignored (this an be traced in the github actions outputs).

![Presentation toc generation](./img/gh-actions-toc-step.png)
