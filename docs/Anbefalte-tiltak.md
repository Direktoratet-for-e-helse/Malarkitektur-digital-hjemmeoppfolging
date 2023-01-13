| Status           | Version | Maturity | Normative level |
| :--------------- | :------ | :------- | :-------------- |
| <span style="background-color:gold">Work in progress</span> | v0.1 | draft | ikke normert |

Denne delen av målarkitekturen skal foreslå tiltak som kan gjennomføres for å understøtte etableringen av datadeling mellom virksomheter innen for behovsområdet DHO. Vi skiller på tiltak knyttet til etablering av felleskomponenter og tiltak som må gjennomføres av hver enkelt virksomhet som ønsker å etablere datadeling for samhandling med andre virksomheter.

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

Digital hjemmeoppfølging og deling av målinger er en annen utprøvingskandidat som er identifisert utover dokumentdeling gjennom kjernejournal. Det er viktig at bruk av felles tillitsmodell prøves ut for en datadelingstjeneste som DHO i tillegg til utprøvingen knyttet til dokumentdeling siden det kan gi viktig kunnskap om hvordan tillitsmodellen fungerer for datadelingsløsninger. Vi vet foreløpig for lite om kravene som stilles til tillitsmodellen knyttet til datadeling selv om hypotesen er at datadeling og dokumentdeling skal løses på samme måte er det viktig å få bekreftet den antakelsen.

### Vurdere fellesløsninger for MTU

Innspill fra aktørene som arbeider med spredning og utprøving av DHO har pekt på to store utfordringer knyttet til etablering av DHO tjenester. Det ene handler om samhandling som behandles i dette dokumentet. Et annet behov som er identifisert er knyttet til tildeling og forvaltning av det tekniske utstyret som skal samle målinger hjemme hos pasienten, ofte omtalt som MTU.

Det er identifisert mange behov knyttet til administrasjon av MTU og bare noen av disse kan dekkes med ren oversikt over hvilket utstyr pasienten har, uavhengig av hvem som har tildelt dette:

* Kjenne til tjenester, ytelser og hjelpemidler og hvilke aktører som har tildelt disse
* Kjenne til om relevant utstyr er tildelt fra andre aktører
* Unngå dobbelt sett av utstyr med overlappende funksjonalitet
* Tilgang til data fra MTU-utstyr
* Tilgang til administrasjon av MTU-utstyr

#### Anbefalte tiltak



## Tiltak knyttet til semantisk samhandling

## Tiltak i hver enkelt virksomhet
