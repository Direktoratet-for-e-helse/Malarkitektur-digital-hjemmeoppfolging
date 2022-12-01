# Testdokumentasjon Målarkitektur-digital-hjemmeoppfølging

Testprosjekt for å se hvordan arkitekturdokumentasjon enklest mulig kan publiseres og vedlikeholdes på Github i regi Direktoratet for e-helse.

* [Generert dokumentasjon for målarkitekturen](https://direktoratet-for-e-helse.github.io/Malarkitektur-digital-hjemmeoppfolging/)

## Verktøy

### Markdown

Ukjent med [Github markdown syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)? Da anbefaler vi [Markdown Editor til Visual Studio](https://marketplace.visualstudio.com/items?itemName=zaaack.markdown-editor)

### VSCode

Kom igang med VSCode og repo fra Github:

For å komme i gang må du installere VSCode og klone repositoriet vårt fra Github til din lokale harddisk. Kloningen trenger du bare å gjøre en gang. Neste gang åpner du kopien fra lokal disk og trykker **Pull changes** for å hente de siste endringene fra serveren/repoet.

> Før du kan klone repoet lokalt må du ha Git installert på PC, det skal bli installert sammen med "Git Extensions" programmet i Firmaportalen.

1. Hente opp Command palette
> View -> Command palette

2. Skriv inn kommandoen: 
> Git: Clone <kbd>Enter</kbd>
3. Lim inn adressen til GitHub repoet:
~~~
https://github.com/Direktoratet-for-e-helse/Malarkitektur-digital-hjemmeoppfolging
~~~
4. Velg en katalog på harddisken du ønsker å klone til (jeg bruker vanligvis C:\Github). <kbd>Select Repository Location</kpd>
5. Trykk <kbd>Open</kbd> i dialogvinduet

Du skal nå få opp katalogstrukturen til repositoriet i fil explorer på venstre side i VSCode.
Husk at endringer du gjør i VSCode skrives til kopien av repoet på lokal disk. Du må commite og pushes endrede filer til repoet (remote) for at dine endringer skal bli synlige for andre.

### OPTIONAL: Enable Git in VSCode

Kanskje må man gjøre dette også før man kan bruke Git i VSCode.

1. Go to File > Preferences
1. Go to Settings
1. Type Git: Enabled in the search bar
1. Make sure that the box is ticked

## Layout

* [just the docs - layout template for Github.io sidene](https://github.com/just-the-docs/just-the-docs)
* [Oversette](https://metamug.com/util/confluence-to-markdown/) confluence sider til markdown

### Forutsetninger *just-the-docs*

* index.md må ligge i rotkatalog på prosjektet?
* markdown filene bør ha just-the-docs metadata

~~~
---
layout: default
title: Innledning
nav_order: 1
---
~~~
