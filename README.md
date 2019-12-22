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

#### Markdownify

```markdown
{% capture markdown %}
* Lorem ipsum dolor sit amet
* Consectetur adipiscing elit
* Integer molestie lorem at massa
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem
{% endcapture %}
{{ markdown | markdownify }}
```

#### Dividers, jump to section, add style to markdown from Liquid

```markdown
---

<a href="#downloads">downloads</a>

{: .text-purple}

{: style="margin-top:100px;"}
```

#### Liquid programming

```html
{% capture icon_links %}
https://maritadante.it|home,
mailto:marita.dante@gmail.com|at,
tel:+390444542197|phone,
tel:+393473194073|mobile,
https://www.facebook.com/bianco.luigi.9|facebook,
https://github.com/maritadante|github
{% endcapture %}

{% assign icon_links = icon_links | split: "," -%}
{%- for icon_link_string in icon_links -%}
{%- assign icon_link = icon_link_string | split: "|" -%}
<a href="{{icon_link[0]}}">
<span class="fa-stack fa-lg">
<i class="fa fa-circle fa-stack-2x"></i>
<i class="fa fa-{{icon_link[1]}} fa-stack-1x" style="color: white;"></i>
</span></a>
{%- endfor %}
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

## TODOs

* transform as much as possible into markdown (starting with sections likely to be edited often)
* host and present high resolution images for art and photos
* improve rendering on mobile (use fluid for book divs, responsive breaks for sliders -- see examples)
* add minisites for each book
* for "Matematica Ragionata", add questions and answers with [accordions](https://raw.githubusercontent.com/cesium/codeweek15/gh-pages/_posts/2000-01-02-activities.md)
