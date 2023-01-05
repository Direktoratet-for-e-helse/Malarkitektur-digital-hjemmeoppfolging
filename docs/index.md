---
layout: default
title: Innledning
nav_order: 1
---

| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
| <span style="background-color:gold">Work in progress</span> | v0.6 | draft  | ikke normert |

Direktoratet for e-helse har et overordnet mål om å øke digital samhandling mellom aktørene i helse- og omsorgssektoren. Det er startet en rekke tiltak innenfor området data- og dokumentdeling. Dette arbeidet er prioritert fordi data- og dokumentdeling er samhandlingsformer som tas i bruk på ulike måter innen stadig nye områder innen helse- og omsorgstjenesten. Hensikten er å sikre en koordinert utvikling av datadeling samt økt bruk i hele sektoren.  

Innen digital hjemmeoppfølging er behovet for datadeling spesielt stort. Pasientene som behandles trenger fortløpende oppfølging av flere virksomheter og omsorgsnivå. Mange tjenestetilbydere ser at eksisterende samhandlingsløsninger ikke understøtter samhandlingsbehovet godt nok.  

## Hva er Digital hjemmeoppfølging

I 2021 ble det i rapport fra de regionale helseforetakene foreslått følgende definisjon

**Digital hjemmeoppfølging innebærer at hele eller deler av et behandlingstilbud foregår uten fysisk kontakt, der dialog og deling av data mellom pasient/bruker og behandler(e) skjer digitalt.**

![Hva er DHO?](img/veikart-DHO.png){ width="500" }

Forslaget til definisjon har til hensikt å romme en bredde av ulike former for digital oppfølging og samhandling mellom pasienten og helsetjenesten. Det skal jobbes videre med definisjonsbeskrivelsen gjennom Nasjonalt velferdsteknologiprogram.

Det er vesentlig at oppfølgingen ikke begrenses til der pasienten bor, men at digital hjemmeoppfølging også skal kunne benyttes andre steder, for eksempel på jobb, skole, institusjon, på reise og hos ulike helseaktører. Pasienten kan i prinsippet oppholde seg hvor som helst fysisk, men likevel kunne nå et avstandsbasert helsetilbud når det er forsvarlig.

## Formålet med målarkitekturen

Målarkitekturen skal være et verktøy for å koordinere innsatsen i sektoren slik at alle aktørene arbeider i samme retning for å løse utfordringer knyttet til digital samhandling ved hjelp av datadeling innen behovsområdet for digital hjemmeoppfølging.

* Muliggjøre arkitekturstyring regionalt, nasjonalt og for andre grupperinger av dataansvarlige gjennom å etablere felles arkitekturmål og beskrive arkitekturmønstre.
  * Målarkitekturen har fokus på utveksling av pasientrapporterte data og etableringen av samhandlingsløsninger for å utveksle disse mellom virksomheter og omsorgsnivå
  * Dokumentere felles arkitekturvalg og anbefalte samhandlingsmønster for DHO
  * Beskrive informasjonstjenester og infrastrukturtjenester som må etableres for å realisere digital samhandling i form av datadeling
* Gi oversikt over behovsbildet for samhandling innen DHO
  * Beskrive behov for informasjon og samhandling på tvers av virksomheter og omsorgsnivå med spesielt fokus på behov knyttet til tjenester der DHO benyttes
* Skal fungere som kommunikasjonsverktøy mot helse- og omsorgstjenesten, leverandører og NHN
  * Benyttes i drøfting og forankring av felles retning for utvikling av samhandlingsløsninger
* Beskrive juridisk mulighetsrom for realisering samhandling ved hjelp av datadeling

## Målgruppe

## Omfang og avgrensninger

!!! note "Målarkitektur for datadeling i helsesektoren"

    Målarkitekturen er en beskrivelse av en fremtidig ønsket situasjon, hvor helsesektoren kan dele strukturerte helseopplysninger på tvers mellom virksomheter og omsorgsnivå i et nasjonalt perspektiv. Det er tatt utgangspunkt i behovene og de lovmessige rettigheter og plikter til innbyggere og helsepersonell. Ut ifra dette er det beskrevet ulike bruksområder for datadeling. Målarkitekturen har fokus på samhandling mellom helsepersonell på tvers av virksomheter og samhandling med innbygger.

Omfanget for målarkitekturen for datadeling innen DHO er avgrenset til å understøtte helsetjenester hvor DHO benyttes aktivt i tjenesteforløpet. Målarkitekturen skal derfor beskrive juridiske, behovsmessige og tekniske rammer for hvordan datadeling innen DHO bør realiseres. Målarkitekturen vil videre peke på nødvendige tiltak for infrastruktur, semantiske spesifikasjoner og foreslåtte realiseringskonsepter for å realisere samhandling i form av datadeling.

![Omfang målarkitektur DHO](img/omfang-malarkitektur.png)

* Det er fokus på tilrettelegging for samhandling mellom virksomheter og omsorgsnivå og samhandling med innbygger
  * Noen av de samme mekanismene kan også benyttes for samhandling internt i en virksomhet, men det er ikke hovedfokuset i dette arbeidet
* Det er fokus på utveksling av strukturert informasjon mellom virksomheter og omsorgsnivå. Høy semantisk samhandlingsevne (hva dataene betyr og hvordan de er definert) er nødvendig
* Det er fokus på primærbruk av data. Sekundærbruk av data er ikke et sentralt tema for dette arbeidet
  * Det antas at utveksling av strukturert informasjon kan være nyttig også knyttet til sekundærbruk innen forskning og kvalitetssikring av helsehjelp
* Velferdsteknologi (tradisjonell trygghets og mestringsteknologi) er ikke en del av omfanget for målarkitekturen for DHO.
  * Behovene knyttet til trygghet og mestring er relativt godt analysert i tidligere arbeid og det er bare små overlapp mellom DHO og trygghet og mestringsområdet
  * Noen teknologiske løsninger og utfordringer er imidlertid sammenfallende med trygghet og mestringsområdet og vil også være en naturlig del av behovsbildet og løsningene som benyttes innen DHO området
* Der viktige infrastrukturtjenester eller semantiske spesifikasjoner ikke eksisterer vil målarkitekturen peke på nødvendige tiltak for å realisere disse
  * Plan for realisering av tiltakene ligger utenfor mandatet til målarkitekturen

### Modenhet

Bruk av datadeling for digital samhandling mellom virksomheter, omsorgsnivå og pårørende/pasient er relativt umodent. Til tross for mange utprøvingsprosjekter i velferdsteknologiprogrammet har arbeidet med samhandling i form av datadeling kommet relativt kort og det er få tjenester som er realisert og tatt i bruk av helsetjenesten. Erfaringsunderalget er derfor lite og anbefalinene knyttet til data deling er derfor beheftet med stor usikkerhet. Det vil være behov for revisjon av anbefalingene etterhvert som flere tjenester blir realisert.

Modenheten er også relativt lav når det gjelder å ta i bruk Digital Hjemmeoppfølging i helsetjenesten. Men her er erfaringsunderlaget bedre etter at flere utprøvingsprosjekter er gjennomført i perioden 2018-2021. En erfaringsoppsummering er publisert av Helsedirektoratet.

* [Digital hjemmeoppfølging - sluttrapport fra nasjonal utprøving 2018-2021](https://www.helsedirektoratet.no/rapporter/digital-hjemmeoppfolging-sluttrapport-fra-nasjonal-utproving-2018-2021)