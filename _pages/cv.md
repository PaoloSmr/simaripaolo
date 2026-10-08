---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<!--
  Per il CV completo in PDF: carica il file nella cartella "files" con il nome cv.pdf
  e il link qui sotto funzionerà da solo.
-->
[Scarica il CV completo (PDF)]({{ base_path }}/files/cv.pdf)

Formazione
======
* [DA COMPLETARE: Dottorato in ..., Università di ..., anno – in corso]
* [DA COMPLETARE: Laurea magistrale in ..., Università di ..., anno]
* [DA COMPLETARE: Laurea triennale in ..., Università di ..., anno]

Esperienze
======
* [DA COMPLETARE: anno–anno: ruolo]
  * [ente]
  * [breve descrizione]

Competenze
======
* [DA COMPLETARE: metodi, software, lingue]

Pubblicazioni
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Interventi
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>

Didattica
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
