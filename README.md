# Testdokumentasjon Målarkitektur-digital-hjemmeoppfølging

Testprosjekt for å se hvordan arkitekturdokumentasjon enklest mulig kan publiseres og vedlikeholdes på Github i regi Direktoratet for e-helse.

* [Generert dokumentasjon for målarkitekturen](https://direktoratet-for-e-helse.github.io/Malarkitektur-digital-hjemmeoppfolging/)

## Bruker

* [just the docs - layout template for Github.io sidene](https://github.com/just-the-docs/just-the-docs)
* [Oversette](https://metamug.com/util/confluence-to-markdown/) confluence sider til markdown

### Anbefaling

Ukjent med [Github markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)? Da anbefaler vi [Markdown Editor til Visual Studio](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor)

## Forutsetninger

* index.md må ligge i rotkatalog på prosjektet?
* markdown filene bør ha just-the-docs metadata

~~~
---
layout: default
title: Innledning
nav_order: 1
---
~~~
