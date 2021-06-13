---
title: "Interventi"
bg: "#2e2e2e"
color: white
icon: img/icone/interventi.jpg
---
## Mostre e Conferenze

{% capture interventi %}
{% include interventi.txt %}
{% endcapture %}

{% capture divs %}
{%- assign interventi = interventi | strip | newline_to_br | split: '<br />' -%}
{%- for intervento_string in interventi -%}

    {%- assign intervento = intervento_string | split: '|' -%}
    <div>
    <img src="{{intervento[0] | strip}}" alt="{{intervento[0] | strip}}" />
    {{intervento[1] | strip  | markdownify}}
    </div>

{%- endfor %}
{% endcapture %}

<div class="carosello grande" id="carosello-interventi-grande" data-slick='{"focusOnSelect": true, "arrows": true, "dots": false, "fade": true, "autoplay": true, "asNavFor": "#carosello-interventi-piccole", "speed": 800, "autoplaySpeed": 4500, "adaptiveHeight": true}'>
{{ divs }}
</div>

<div class="carosello piccole" id="carosello-interventi-piccole" data-slick='{"variableWidth": true, "centerMode": true, "focusOnSelect": true, "infinite": true, "arrows": true, "dots": false, "asNavFor": "#carosello-interventi-grande"}'>
{{ divs }}
</div>
