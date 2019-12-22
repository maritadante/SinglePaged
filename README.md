# Sito personale di Marita Dante

Sito personale di Marita Dante.
Tutti i diritti riservati.

## Collegamenti

* Sito: [maritadante.it](https://maritadante.it/)
* Github: [home](https://github.com/maritadante), [sito](https://github.com/maritadante/maritadante.github.io), [template](https://github.com/t413/SinglePaged)
* [Github pages documentation](https://help.github.com/en/github/working-with-github-pages)
* [Matematica Ragionata wordpress](https://matematicaragionata.wordpress.com/curriculum)

## Temi ed esempi

* [Jekyll Themes](http://jekyllthemes.org)
* [Portfolio theme](http://bogoli.github.io/-folio/)
* [Prologue theme](https://chrisbobbe.github.io/jekyll-theme-prologue)

## TODOs

* transform as much as possible into markdown (starting with sections likely to be edited often)
* host and present high resolution images for art and photos
* improve rendering on mobile (use fluid for book divs, responsive breaks for sliders -- see examples below)
* add mini, single page landing sites for each book
* for "Matematica Ragionata", add questions and answers with [accordions](https://raw.githubusercontent.com/cesium/codeweek15/gh-pages/_posts/2000-01-02-activities.md)

## Documentation

* Markdown cheatsheets: [soshace](https://dev.to/soshace/markdown-cheat-sheet-definitive-guide-to-markdown-markdown-resources-n15), [adam](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet), [sindresorhus](https://sindresorhus.com/github-markdown-css/), [github](https://guides.github.com/features/mastering-markdown/)
* [Styling Markdown](https://digitaldrummerj.me/styling-jekyll-markdown/)
* [Kramdown quickreference](https://kramdown.gettalong.org/quickref.html)
* [Jekyll layouts](https://jekyllrb.com/docs/layouts/)
* [Google fonts](https://fonts.google.com/)

## Local development

* Run: **jekyll serve -w**
* [Jekyll localhost](http://localhost:4000/)

## Examples

#### Dividers, jump to section, add style to markdown from Liquid

```markdown
---

<a href="#downloads">downloads</a>

{: .text-purple}

{: style="margin-top:100px;"}
```

#### Responsive sliders

```javascript
$('.partners').slick({
  slidesToShow: 2,
  responsive: [
  {
    breakpoint: 976,
    settings: {
      slidesToShow: 1,
      slidesToScroll: 1
    }
  }]
});
```

#### Tabular data

```markdown
user                  |      group     |others
:---------------------:|:--------------:|:------:
7                     |       5        |  4
read + write + execute | read + execute | read
```
