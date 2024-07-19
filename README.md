
# Development presentations
This Github project contains the developpers' presentations. 

## Technologies
The presentations are written in <a href="https://www.markdownguide.org/cheat-sheet/" target="_blank">Markdown</a> and is based on <a href="https://pages.github.com/" target="_blank">Github pages</a>, <a href="https://docs.github.com/fr/actions" target="_blank">Github actions</a> and <a href="https://marp.app/" target="_blank"> Marp</a>.

## New presentations
**Location :** The new presentations should be created under the directory docs.<br/>
**Naming convention :** The file name template is ` yyyy-mm-dd-the-new-presentation.md`.<br/><br/>
A TOC can be generated in a presentation by inserting the comments:
```
<!--ts-->
<!--te-->
```
The titles of level 1 an 2 are used to generate the table of content via the utilitary <a href="https://github.com/ekalinin/github-markdown-toc" target="_blank"> github-markdown-toc</a>.
gh-md-toc is executed vi the Github actions, step Toc generation. If the file does not contain the comments for the TOC it is ignored (this an be traced in the github actions outputs).

![Presentation toc generation](./img/gh-actions-toc-step.png)
*Toc generation output in Github actions*

## Presentations list.
A main TOC (a presentations list) is generated an inserted in the index file via the Github actions. It uses the script [generate-toc.sh](https://github.com/avenirs-esr/presentations/blob/c78d67f3ce3eaa1c33e7458a8cb6a57f60d84f6a/scripts/generate-toc.sh). 

The insertion slot is determined by the comment
`<!-- {{TOC}} -->` in the file [index.template.md](https://github.com/avenirs-esr/presentations/blob/3d6d95017c072d0efff178592fee46b453419599/index.template.md?plain=1#L52).

The title is extracted from the file name or should be set via the optional property [avenirs-toc](https://github.com/avenirs-esr/presentations/blob/3d6d95017c072d0efff178592fee46b453419599/docs/2024-03-12-Point_d_etape_devs.md?plain=1#L4) in the front matter.
