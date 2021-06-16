# Sito personale di Marita Dante

Sito personale di Marita Dante.
Tutti i diritti riservati.

## Collegamenti

* Sito: [maritadante.it](https://maritadante.it/)
* Github: [home](https://github.com/maritadante), [sito](https://github.com/maritadante/maritadante.github.io), [template](https://github.com/t413/SinglePaged)
* [Guida Markdown](https://informaticabrutta.it/markdown-guida/)
* [Github pages documentation](https://help.github.com/en/github/working-with-github-pages)

## Temi ed esempi

* [Jekyll Themes](http://jekyllthemes.org)
* [Portfolio theme](http://bogoli.github.io/-folio/)
* [Prologue theme](https://chrisbobbe.github.io/jekyll-theme-prologue)

## TODOs

* transform as much as possible into markdown (starting with sections likely to be edited often)
* improve rendering on mobile (use fluid for book divs, responsive breaks for sliders -- see examples below)
* for "Matematica Ragionata", add questions and answers with [accordions](https://raw.githubusercontent.com/cesium/codeweek15/gh-pages/_posts/2000-01-02-activities.md) See also: [Matematica Ragionata wordpress](https://matematicaragionata.wordpress.com/curriculum)

## Documentation

* Markdown cheatsheets: [soshace](https://dev.to/soshace/markdown-cheat-sheet-definitive-guide-to-markdown-markdown-resources-n15), [adam](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), [sindresorhus](https://sindresorhus.com/github-markdown-css/), [github](https://guides.github.com/features/mastering-markdown/)
* [Styling Markdown](https://digitaldrummerj.me/styling-jekyll-markdown/)
* [Kramdown quickreference](https://kramdown.gettalong.org/quickref.html)
* [Jekyll layouts](https://jekyllrb.com/docs/layouts/)
* [Google fonts](https://fonts.google.com/)

## Local development

* Run: ```export PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH"; jekyll serve -w```
* [Jekyll localhost](http://localhost:4000/)

## Examples

#### Dividers, jump to section, add style to markdown from Liquid

```markdown
---

<a href="#downloads">downloads</a>

{: .text-purple}

{: style="margin-top:100px;"}
```

#### Tabular data

```markdown
user                  |      group     |others
:---------------------:|:--------------:|:------:
7                     |       5        |  4
read + write + execute | read + execute | read
```
