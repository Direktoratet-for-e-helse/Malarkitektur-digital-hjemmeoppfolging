---
layout: default
title: Innledning
nav_order: 1
---

| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
| <span style="background-color:gold">Work in progress</span> | v0.6 | draft  | ikke normert |

## Bakgrunn

Direktoratet for e-helse har et overordnet mål om å øke digital samhandling mellom aktørene i helse- og omsorgssektoren. Det er startet en rekke tiltak innenfor området data- og dokumentdeling. Dette arbeidet er prioritert fordi data- og dokumentdeling er samhandlingsformer som tas i bruk på ulike måter innen stadig nye områder innen helse- og omsorgstjenesten. Hensikten er å sikre en koordinert utvikling av datadeling samt økt bruk i hele sektoren.  
Innen digital hjemmeoppfølging er behovet for datadeling spesielt stort. Pasientene som behandles trenger fortløpende oppfølging av flere virksomheter og omsorgsnivå. Mange tjenestetilbydere ser at eksisterende samhandlingsløsninger ikke understøtter samhandlingsbehovet godt nok.  
Målarkitektur for datadeling ble publisert..  
dette arbeidet baserer seg på målarkitektur for datadeling...  

### Digital hjemmeoppfølging

*Digital hjemmeoppfølging er nye tjenester under utvikling hvor deler av helse- og omsorgstjenesten kan flyttes hjem til innbygger ved hjelp av teknologi.*

Begrepet tolkes ulikt, men vil som regel inkludere oppfølging basert på egenmåling og egenrapportering, nettbasert behandling, hjemmesykehus, medisinsk avstandsoppfølging, videokonsultasjon og bruk av visse typer velferdsteknologi, som for eksempel digitalt tilsyn og medisindispensere.

Det er vesentlig at oppfølgingen ikke begrenses til der pasienten bor, men at digital hjemmeoppfølging også skal kunne benyttes andre steder, for eksempel på jobb, skole, institusjon, på reise og hos ulike helseaktører.

Pasienten kan i prinsippet oppholde seg hvor som helst fysisk, men likevel kunne nå et avstandsbasert helsetilbud når det er forsvarlig.

## Formålet med målarkitekturen

Målarkitekturen skal være et verktøy for å koordinere innsatsen i sektoren slik at alle aktørene arbeider i samme retning for å løse samhandlingsutfordringene.

* Definere felles arkitekturmål for samhandling innen DHO
    * Målarkitekturen har fokus på pasientrapporterte data og samhandlingsløsninger for å utveksle disse mellom virksomheter og omsorgsnivå
  * Målarkitekturen skal fungere som et verktøy for å koordinere innsatsen i sektoren for å etablere datadelingsløsninger innen DHO området
  * Dokumentere felles arkitekturvalg og anbefalte samhandlingsmønster for DHO
  * Beskrive informasjonstjenester og infrastrukturtjenester som må etableres for å realisere samhandlingen
* Gi oversikt over behovsbildet
  * Beskrive behov for informasjon og samhandling på tvers av virksomheter og omsorgsnivå
* Skal fungere som kommunikasjonsverktøy mot helse- og omsorgstjenesten, leverandører og NHN
  * Benyttes i drøfting og forankring av felles retning for utvikling av DHO løsninger
* Beskrive juridiske problemstillinger knyttet til DHO
  * Beskrive det juridiske handlingsrommet for etablering av datadelingsløsninger i helsesektoren

## Målarkitektur for samhandling innen digital hjemmeoppfølging inneholder

* Dokumenterer felles arkitekturvalg og samhandlingsmønster som benyttes i DHO
* Behov for informasjon og samhandling for å understøtte tjenesten
  * Inkludert bruk av eksisterende eller planlagte informasjonstjenester
* Dokumentere aktører som skal samhandle og samhandlingsmønstre som fungerer mellom disse
  * Oppsummere erfaringer
* Informasjonstjenester og infrastrukturtjenester som kan ivareta behovene
  * Infrastrukturtjenester (NHN) og tjenester som virksomhetene selv må implementere
    * Peke på nødvendige fellestjenester, infrastruktur og integrasjonspunkter inn i egen organisasjon
  * Gap mellom AS-IS og TO-BE, tiltak som utfyller gapet
* Behov for andre normerende produkter (Semantisk nivå, tillitstjenester, hvordan etablere infrastrukturtjenester i virksomheten)
* Overordnede juridiske avklaringer

## Målgruppe

## Omfang og avgrensninger

Målarkitekturen skal være et verktøy for å koordinere innsatsen i sektoren slik at aktørenen arbeider i samme retning for å løses samhandlingsutfordringene. Den skal blant annet inneholde hvilke samhandlingstjenester som skal tilbys nasjonalt. Det er derfor gjort noen avgrensninger i forhold til de behovene som analyseres i arbeidet med målarkitektur for samhandling innen DHO.

* Det er fokus på tilrettelegging for samhandling mellom virksomheter og omsorgsnivå og samhandling med innbygger
  * Noen av de samme mekanismene kan også benyttes for samhandling internt i en virksomhet, men det er ikke hovedfokuset i dette arbeidet
* Det er fokus på utveksling av strukturert informasjon mellom virksomheter og omsorgsnivå. Høy semantisk samhandlingsevne (hva dataene betyr og hvordan de er definert) er nødvendig
* Det er fokus på primærbruk av data. Sekundærbruk av data er ikke et sentralt tema for dette arbeidet
  * Det antas at utveksling av strukturert informasjon kan være nyttig også knyttet til sekundærbruk innen forskning og kvalitetssikring av helsehjelp
* Velferdsteknologi (tradisjonell trygghets og mestringsteknologi) er ikke en del av omfanget for målarkitekturen for DHO.
  * Behovene knyttet til trygghet og mestring er relativt godt analysert i tidligere arbeid og det er bare små overlapp mellom DHO og trygghet og mestringsområdet
  * Noen teknologiske løsninger og utfordringer er imidlertid sammenfallende med trygghet og mestringsområdet og vil også være en naturlig del av behovsbildet og løsningene som benyttes innen DHO området
