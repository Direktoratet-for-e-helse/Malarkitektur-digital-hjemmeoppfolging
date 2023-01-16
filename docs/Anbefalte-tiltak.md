| Status           | Version | Maturity | Normative level |
| :--------------- | :------ | :------- | :-------------- |
| <span style="background-color:gold">Work in progress</span> | v0.1 | draft | ikke normert |

Denne delen av målarkitekturen skal foreslå tiltak som kan gjennomføres for å understøtte etableringen av datadeling mellom virksomheter innen for behovsområdet DHO. Vi skiller på tiltak knyttet til etablering av felleskomponenter og tiltak knyttet til semantisk samhandling.

## Tiltak knyttet til etablering av felleskomponenter

### Etablering av PIL

[Målarkitektur for datadeling i helse og omsorgssektoren](https://www.ehelse.no/standardisering/standarder/malarkitektur-for-datadeling-i-helse-og-omsorgssektoren) peker på nødvendigheten av å etablere pasientinformasjonslokalisator for å understøtte datadeling basert på distribuert lagring og etablering av grensesnitt for å avgi data. Målarkitektur for datadeling slår også fast at det ikke eksisterer 

!!! quote "Pasientinformasjonslokalisator"

    Det er i en rekke situasjoner tilknyttet datadeling behov for å kunne fremskaffe en oversikt over hvem som har en pasientjournal for en gitt pasient. 
    ...
    Et slikt register bør etableres som en felleskomponent hvor det fremgår hvem som har helseopplysninger om en gitt pasient. Vi har valgt å kalle denne felleskomponenten for pasientinformasjonslokalisator, forkortet til PIL.

#### Status for etablering av PIL - januar 2023

Det eksisterer idag ikke noen tiltak knyttet til å etablere felleskomponent for PIL i samhandlingsinfrastrukturen for helsesektoren

#### Anbefalt tiltak

Spredning av DHO og understøtte behov for datadeling på tvers av mange virksomheter innenfor en region er avhengig av PIL for å fungere effektivt. Det mangler imidlertid mye arbeid før PIL kan etableres som en felleskomponent i samhandlingsinfrastrukturen:

* Utarbeide et konsept for PIL som innenfor gjeldende rett, basert på desentralisert modell
* Alternativt utarbeide forskrift som regulerer behandlingsgrunnlaget for PIL informasjon i en sentralisert løsning
* Planlegge arbeidet med etablering og innføring av PIL
* Etablere PIL som en felleskomponent i samhandlingsinfrastrukturen for helsesektoren

### Felles tillitsmodell for datadeling

!!! quote ""

    Helsesektorens tillitsrammeverk definerer spilleregler og løsninger som virksomhetene som skal samhandle må akseptere og ta i bruk, slik at virksomheten kan få tilgang til helseopplysninger digitalt på en sikker, lovlig og effektiv måte.

#### Status for etablering av felles tillitsmodell - januar 2022

Det gjennomføres arbeid knyttet til å etablere felles tillitsmodell i forbindelse med utbredelse av dokumentdeling i regi av program digital samhandling. Norsk Helsenett etablerer felleskomponenter for felles tillitsmodell og løsningen skal prøves ut og videreutvikles i forbindelse med Dokumentdeling gjennom kjernejournal.

#### Anbefalt tiltak

I tillegg til dokumentdeling gjennom kjernejournal er digital hjemmeoppfølging og deling av målinger identifisert som utprøvingskandidat for felles tillitsmodell. Sett fra helsetjenesten som prøver ut DHO sitt perspektiv er viktig at bruk av felles tillitsmodell prøves ut for datadelingstjenester som DHO i tillegg til utprøvingen knyttet til dokumentdeling, siden det kan gi viktig kunnskap om hvordan tillitsmodellen fungerer for datadelingsløsninger. Vi vet foreløpig lite om kravene som stilles til tillitsmodellen knyttet til datadeling og selv om hypotesen er at tillitsmodellen for datadeling og dokumentdeling fungere likt er det viktig å få bekreftet den antakelsen.

Det anbefales at enkelte DHO tjenester som etablerer datadeling mellom virksomheter tar i bruk felles tillitsmodell og fellskomponenter som felles tillitsanker. 

### Vurdere fellesløsninger for MTU

Innspill fra aktørene som arbeider med spredning og utprøving av DHO har pekt på to store utfordringer knyttet til etablering av DHO tjenester. Det ene handler om samhandling som behandles i dette dokumentet. Et annet behov som er identifisert er knyttet til tildeling og forvaltning av det tekniske utstyret som skal samle målinger hjemme hos pasienten, ofte omtalt som MTU.

Det er identifisert mange behov knyttet til administrasjon av MTU og bare noen av disse kan dekkes med ren oversikt over hvilket utstyr pasienten har, uavhengig av hvem som har tildelt dette:

* Kjenne til tjenester, ytelser og hjelpemidler og hvilke aktører som har tildelt disse
* Kjenne til om relevant utstyr er tildelt fra andre aktører
* Unngå dobbelt sett av utstyr med overlappende funksjonalitet
* Tilgang til data fra MTU-utstyr
* Tilgang til administrasjon av MTU-utstyr

#### Anbefalt tiltak

Det anbefales at det settes igang arbeid som gjør det mulig for flere virksomheter å høste informasjon fra det samme utstyret, uavhengig av hvem som har tildelt utstyret. Det må først gjøres et mer grundig behovsarbeid og det må sannsynliggjøres at en slik løsning gir tilstrekkelig verdi til at det er formålstjenlig å etablere felles infrastruktur for å ivareta behovet.

## Tiltak knyttet til semantisk samhandling

Kapitelet som beskriver [konsepter for realisering](Konsepter-realisering.md) av datadeling mellom virksomheter og omsorgsnivå peker på nødvendigheten av felles semantiske spesifikasjoner for å understøtte distribuerte konsepter. Det er behov for semantiske spesifikasjoner ved etablering av sentrale/nasjonale løsninger også, men dette vil realiseres gjennom grensesnittspesifikasjonene i den sentrale løsningen.

### Felles semantisk rammeverk for datadeling og DHO

Utprøving og spredningsprosjektene som gjennomføres nå baserer seg på et lite sett [HL7 FHIR](https://hl7.org/fhir/) profiler som beskriver det semantiske innholdet i målinger som kan utveksles mellom virksomhetene. Profilene beskriver i hovedsak tre forhold knyttet til utveksling av informasjon mellom virksomhetene:

* Overordnet brukertilfelle profilene understøtter
* Hvilken informasjon som er minimum for at informasjonen skal vær nyttig
* Regler for informajsonsinnhold i de spesifikke informasjonselementene
  * Inkluderer regler om bruk av felles terminologi og kodeverk

Vi tror det er nødvendig at det eksisterer felles beskrivelse av dette på tvers av virksomheter for at datadeling skal fungere på en god måte, dette er uavhengig av om distribusjonen av data baserer seg på en sentral eller distribuert modell. Ved en distribuert modell er det imidlertid et ufravikelig krav at det er felles regler for hvordan informasjonen skal utformes, ellers vil etablering av oppslagstjenester mot mange ulike grensesnitt bli en uoverstigelig oppgave hvor utviklerne må forholde seg til en rekke typer semantiske spesifikasjoner. Integrasjon mot bakenforligende systemer vil også bli svært komplisert.

### Utestående arbeid knyttet til semantisk samhandling

Foreløpig er det bare et fåtall profiler som er utviklet, disse har også sett lite praktisk bruk og er implementert i få løsninger. Det er viktig at profilene videreutvikles i tre retninger:

* Kvantitet - det er få brukertilfeller som er dekket av eksisterende profiler, det må testes og utvikles flere for å dekke flere brukertilfeller og flere typer informasjonstjenester
* Kvalitet - profilene må implementeres i flere løsninger og testes i praktisk bruk i større grad for å kvalitetsikre at innholdet er tilstrekkelig for praktisk klinisk bruk og teste at integrasjon mot mange bakenforliggende løsninger kan gjennomføres
* Innhold - dagens profiler beskriver informasjonsinnholdet, men også lovlige søkeparametere bør detaljeres i neste versjon av profilene. På denne måten kan man sikre at datadelingstjenestene tilbyr den samme søkefunksjonaliteten uavhengig av hvem som implementerer grensesnittene

### Anbefalte tiltak

Det anbefales tiltak knyttet til alle de tre retningene som beskrives under [utestående arbeid](#utestående-arbeid-knyttet-til-semantisk-samhandling) men Kvantitet for å dekke flere brukertilfeller og kvalitet for å teste eksisterende profiler bedre haster mest.