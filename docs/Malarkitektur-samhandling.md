---
layout: default
title: Målarkitektur samhandling DHO
nav_order: 7
---

| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
| <span style="background-color:gold">Work in progress</span> | v0.8 | review  | ikke normert |

## Samhandling mellom helsepersonell på tvers av virksomheter

Direktoratet for e-helse publiserte i mars 2021 [Målarkitektur for datadeling](https://www.ehelse.no/standardisering/standarder/malarkitektur-for-datadeling-i-helse-og-omsorgssektoren/_/attachment/inline/a5a908cd-5054-4d21-8eaf-8b795dcb25ea:761793d5dd6b6a1f2b9dd334a44e3a754d5b88e6/M%C3%A5larkitektur%20for%20datadeling%20i%20helse-%20og%20omsorgssektoren%20(HITR%201231_2021).pdf) som tar frem "samhandling mellom helsepersonell på tvers av virksomheter" som et brukstilfelle, men som <!--kanskje det skulle være et IKKE her?-->ble behandlet i første versjon <!--Hva viser denne første versjon til. Forstå ikke -->siden modenheten den gang var for lav.

Arbeid med målarkitektur for DHO skal ta brukstilfellet "samhandling mellom helsepersonell på tvers av virksomheter" videre, og dette vil bli en del av den overordnede målarkitekturen for datadeling for helsesektoren. Slik beskrives brukstilfellet i målarkitektur fra datadeling:

"Dette bruksområdet dekker brukstilfeller som i hovedsak dekker behovet for at helsepersonell i ulike virksomheter må samhandle for å yte best mulig helsehjelp.

Virksomheter som yter helsehjelp har en plikt til å samarbeide om behandling og forebygging av sykdom hos innbyggere. Det ligger som en forutsetning for godt samarbeid at aktørene må samarbeide om behandlingsplaner og andre helseopplysninger. Samarbeidet kan inkludere deling av dokumentasjon ved hjelp av datadeling fra den ene virksomheten til den andre, og kan også inkludere digitalisert samarbeid om pasientforløp på tvers av virksomheter. For mer avanserte samarbeidsformer rundt en pasient vil ikke meldings- og dokumentutveksling være tilstrekkelig for å kunne lage fleksible og gode samarbeidsløsninger. Her vil samarbeidsprosesser og arenaer kreve datadeling der aktørene kan samarbeide om både strukturerte dokumenter og mindre informasjonselementer.

Dette bruksområdet <!--peker bruksområde tilbake på målarkitetkuren) Spør fordi bruksområde og brukstilfelle ikke er begrep jeg vansligvis benytter-->må sees i sammenheng med de nasjonale tiltakene som for eksempel dokumentdeling via Kjernejournal, Akson journal og Helseplattformen som skal løse hoveddelen av behovet for samhandling ved å ha en felles journal. Disse tiltakene vil redusere antall løsninger som det må lages samhandlingsfunksjoner som benytter datadeling på tvers.
  
Det er ulik tidshorisont på når disse løsningene er realisert og tatt i bruk. Det vil derfor være behov for å ta i bruk datadeling også frem til disse løsningene er realisert og tatt i bruk.  
Behovsanalysen til konseptvalgutredningen for nasjonal journalløsning for kommunal helse og omsorgstjeneste beskriver [behovene for samhandling i detalj \[7\]](https://ehelse.no/strategi/akson/_/attachment/download/991f83c3-be61-4556-9df6-44e8430ecf8c:c10adb76b95e679fb5857fec60e5c57650ead80b/Vedlegg%20A%20Behovsanalyse%20Nasjonal%20l%C3%B8sning%20for%20kommunal%20helse-%20og%20omsorgstjeneste.pdf).
  
Dette bruksområdet dekker samhandling gjennom datadeling mellom aktører i ulike helseregioner og mellom aktører i helseregioner og den kommunale helse- og omsorgstjenesten inkludert fastleger. Målarkitekturen for dette bruksområdet trenger mer arbeid og vi har valgt å ikke beskrive arkitekturen nærmere i denne versjonen av dokumentet." 

## Kapabilitetskart Konsumere (hendelser), Slå opp og Oppdatere

Modellen viser overordnet kapabilitetskart for prosessene Konsumere informasjon, Vurdere og gjennomføre tiltak, Produsere informasjon og Dele informasjon. Dette er prosesser som er knyttet til Konsumenter (og produsenter) som integrerer mot andre aktører sine tjenester for tilgang til informasjon eller som ønsker å oppdatere informasjon de har produsert i informasjonstjenester som tilbys av andre aktører. Vi har identifisert at det mest relevante samhandlingsmønsteret for informasjonsbehovene knyttet til DHO er "Slå opp", men gode alternativer kan være å konsumere hendelsesstrømmer. For å oppdatere felles informasjonstjenester (for eksempel felles behandlingsplan) vil "Oppdatere" best dekke behovet. For prosesser hvor det er behov for bestilling og henvisning til tjenester som tilbys av andre aktører vil imidlertid sende/motta være foretrukket samhandlingsform.

![Kapabilitetskart prosess](img/kapabilitetskart-prosess.png)

Det er identifisert noen grunnleggende kapabiliteter som må gå på tvers av de overbyggende, dette er dialog, sikkerhet og tillitsmodell.

Kjernekapabilitetene må være tett knyttet til og integrert med den kliniske prosessen som handler om å identifisere og gjennomføre tiltak som en del av pasientbehandlingen, men omfatter også produksjon av informasjon. Dette innebærer både selve dokumentasjonen av hva som gjennomføres, målinger og resultater. Det er også tatt med nødvendige kapabiliteter som handler om å generere metadata og lagring av dokumentasjonen i en egnet form for viderebehandling og deling.

### Kapabiliteter knyttet til tiltak og dokumentasjon

Evnene i denne tabellen er tett knyttet opp mot å understøtte vurdering og gjennomføring av tiltak og dokumentasjon av tiltak som utføres som en del av behandlingen av pasient.

<table class="wrapped confluenceTable"><colgroup><col><col><col></colgroup><tbody><tr><th class="confluenceTh">Kapabilitet</th><th class="confluenceTh">Definisjon</th><th class="confluenceTh">Eksempel</th></tr><tr><td class="confluenceTd"><p>Informasjonsbehandling</p></td><td class="confluenceTd">Sammenstille og tolke informasjon fra interne og eksterne systemer</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Visning</td><td class="confluenceTd">Vise informasjonen på en måte som er nyttig for kliniker</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Dokumentere</td><td class="confluenceTd">Dokumentere gjennomførte tiltak og begrunnelsen for tiltaket</td><td class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Produsere metadata</td><td colspan="1" class="confluenceTd">Produsere metadata som beskriver produsert dokumentasjon</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Lagring</td><td colspan="1" class="confluenceTd">Lagre informasjon (dokumentasjon og metadata)</td><td colspan="1" class="confluenceTd"><br></td></tr></tbody></table>

### Tverrgående kapabiliteter

Evnene i denne tabellen er ikke knyttet opp mot noen spesielle deler av prosessen, siden alle deler av prosessen har behov for disse.

<table class="wrapped confluenceTable"><colgroup><col><col><col></colgroup><tbody><tr><th class="confluenceTh">Kapabilitet</th><th class="confluenceTh">Definisjon</th><th class="confluenceTh">Eksempel</th></tr><tr><td class="confluenceTd">Dialog</td><td class="confluenceTd">Understøtte løpende dialog mellom helsepersonell</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Sikkerhet</td><td class="confluenceTd">Ivareta sikker informasjonsutveksling, informasjonsbehandling, tilgangsstyring og personvern</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Tillit</td><td class="confluenceTd">Stole på at informasjon kan utveksles med andre aktører</td><td class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Grunndata</td><td colspan="1" class="confluenceTd">Understøtte behov for tilgang til grunndata i forbindelse med samhandling og pasientbehandling. Grunndata omfatter informasjon om Person, Helsepersonell og Virksomhet.</td><td colspan="1" class="confluenceTd"><br></td></tr></tbody></table>

### Kapabiliteter knyttet til samhandling

Evnene er knyttet til bruk av organisatoriske samhandlingsformer for å utveksle informasjon mellom aktører.

<table class="wrapped confluenceTable"><colgroup><col><col><col></colgroup><tbody><tr><th class="confluenceTh">Kapabilitet</th><th class="confluenceTh">Definisjon</th><th class="confluenceTh">Eksempel</th></tr><tr><td class="confluenceTd">Konsumere hendelsesstrøm</td><td class="confluenceTd">Konsumere hendelser fra en hendelsesstrøm</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Publisere (hendelser)</td><td class="confluenceTd">Publisere hendelser til en hendelsesstrøm</td><td class="confluenceTd"><br></td></tr><tr><td class="confluenceTd">Søk og oppslag (innhente data)</td><td class="confluenceTd">Søke og slå opp informasjon gjennom en <span class="inline-comment-marker" data-ref="9b23afed-5ffd-4399-b2ea-2388ea19eb7c">datadelingstjeneste</span></td><td class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd"><span class="inline-comment-marker" data-ref="c4011089-4276-4fba-a61f-85eefff652da">Tilgjengeliggjøring</span></td><td colspan="1" class="confluenceTd">Evnen til å gjøre data tilgjengelig for aktører utenfor egen virksomhet med eller uten krav til innlogget bruker ved hjelp av datadeling. Tilgangsstyring inngår her. Avgjøre h<span class="inline-comment-marker" data-ref="c1287658-7cf4-4576-acaf-2a02016af69e">vilken informasjon som skal deles med andre gjennom en datadelingstjeneste</span>.</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Tilgjengeliggjøre data</td><td colspan="1" class="confluenceTd">Evnen til å gjøre data tilgjengelig for aktører utenfor egen virksomhet.</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Tilgjengeliggjøre API</td><td colspan="1" class="confluenceTd">Prosessen med å tilby data gjennom et API til aktører utenfor egen virksomhet.</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Få tilgang til data</td><td colspan="1" class="confluenceTd">Evnen til å skaffe seg tilgang til tilbudte data fra annen aktør.</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Finne relevante data</td><td colspan="1" class="confluenceTd">Evnen til å finne kilder for informasjon om spesifikke kategorier eller personer.</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Avgi data</td><td colspan="1" class="confluenceTd">Utlevere data basert på søk og oppslag</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Oppdatering av masterdata</td><td colspan="1" class="confluenceTd">Oppdatere delt informasjon i en datadelingstjeneste</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Sende</td><td colspan="1" class="confluenceTd">Sende informasjon til en spesifikk mottaker</td><td colspan="1" class="confluenceTd"><br></td></tr><tr><td colspan="1" class="confluenceTd">Motta</td><td colspan="1" class="confluenceTd">Motta informasjon fra en spesifikk mottaker</td><td colspan="1" class="confluenceTd"><br></td></tr></tbody></table>

Nødvendige komponenter
----------------------

*   Beskrive komponentene hvilke kapabiliteter de skal realisere
*   Hvem har ansvar for hvilke komponenter (felles/aktører) og hvordan forvaltes disse
    *   Grensesnitt mellom komponentene og forvaltning av disse
*   Lakmustest: Mappe komponentene mot løsningsarkitekturen som er beskrevet for utprøvingene (Oslo, Bodø og Larvik)

### Samhandlingstjenester

Tjenester som det er behov for å realisere samhandlingsevnene. Totalbildet vises i figuren under.

![Samhandlingstjenester](img/213877779.png)

### Tillitstjenester og tjenstlig behov

Juridiske avklaringer i forbindelse datadeling sier at ved oppslag mot kilde/datatilbyder så må konsumentens (sluttbruker) sitt tjenstlige behov dokumenteres overfor datatilbyder før data utleveres. Det eksisterer ikke mekanismer for å håndtere dette i infrastrukturen i dag, verken i sikkerhetsbilletten (må utvides) eller andre tillitsskapende tjenester.

### Samhandlingsformer

Behovet for samhandling i DHO løses best ved å benytte flere [samhandlingsformer](https://confluence.ehelse.no/display/DH/Organisatoriske+samhandlingsformer) om hverandre der ulike samhandlingsformer svarer ut ulike informasjonsbehov og har ulike roller i forhold til behandlingsforløpet. Det eksisterer i dag utstrakt bruk samhandlingsformen sende og motta spesielt knyttet til rekvisisjon, henvisning, svar og epikrise. Dette er ikke hovedfokuset i forbindelse med å utvikle samhandlingen knyttet til DHO da dette er samhandlingsformer og prosesser som er veletablert i tjenesten i dag men som ikke i tilstrekkelig grad understøtter behovene knyttet til DHO og sammensatte behandlingsforløp, hvor ulike virksomheter og omsorgsnivå følger opp pasienten.

### Informasjonstjenester og komponenter - knyttet til API management, sikkerhet og tillitstjenester

Det er identifisert et antall nødvendige informasjonstjenester som er nødvendige for å støtte behovene og realisere evnene som trengs for å understøtte deling av informasjon mellom virksomheter og behandlingsnivå. I tillegg er det behov for tjenester knyttet til tilgjengeliggjøring, oppdaging av API identifisert i målarkitektur for datadeling som har hovedformål å legge til rette for datadeling ved bruk av  API teknologi. Beskrivelsen av behovene innenfor dette området, frem til faktisk datautveksling er godt behandlet i målarkitektur i datadeling og vil ikke gjentas her. Det er noen problemstillinger knyttet til å faktisk understøtte utvekslingen av, bruken av og produksjonen av informasjon som ikke er behandlet i detalj i den arkitekturen og det er denne delen av prosessen vi ser nærmere på i forbindelse med DHO.

![](img/211158301.png)

### Tilgjengeliggjøring

Tilgjengeliggjøring av API og hvilke programvarekomponenter det er behov for i den delen av prosessen som omhandler registrering, avtaler og tildele tilganger er godt behandlet i målarkitektur for datadeling, vi vil ikke diskutere denne delen av prosessen ytterligere her. Prosessen knyttet til å etablere og dokumentere API er nærmere beskrevet gjennom beskrivelsen av prosessene for å etablere API, få tilgang til data og finne relevante data.

![Tilgjengeliggjøring](img/213877320.png)

Prosessen knyttet til etablere API for ekstern tilgang til informasjon fra virksomheten er ikke belyst i målarkitekturen for datadeling. _Etablere API_ er ment å dekke den delen av prosessen som foregår før informasjon faktisk kan tilgjengeliggjøres fra en virksomhet til en annen og handler om prosessen knyttet til å vurder hvilken informasjon som skal tilgjengeliggjøres, tilrettelegge for at denne informasjonen kan tilgjengeliggjøres for andre virksomheter (unntatt sikkerhet og tilgangstyring) og etableringen av funksjonalitet for å avgi informasjonen på en effektiv måte gjennom eksternt tilgjengelige funksjonskall, samt å dokumentere de tilgjengelige grensesnittene.

Vanligvis vil reglene for ekstern tilgang etableres som automatiserte uttrekk fra eksisterende datakilder eller prosesser med fastsatte rammer for hvilken informasjon og metadata som skal være tilgjengelig for eksterne virksomheter. Selve tilgangen etableres ofte ved å etablere en egen løsning for persistering av informasjon som skal være tilgengelig for eksterne funksjonskall. Den eksternt tilgjengelige funksjonen utvikles basert på dette og må gi eksterne virksomheter mulighet til effektive og gode søk etter informasjon slik at konsumenten får dekket sitt behov for gjenbruk av informasjon samtidig som krav til personvern og dataminimering ivaretas. De eksternt tilgjengelige funksjonene dokumenteres vanligvis i API dokumentasjon som publiseres for konsumentene.

#### Etablere API

Prosessen for å Etablere API knyttet til intern dataflyt og eksterne fagsystemer og mellomvare.

![Etablere API](img/217121447.png)

### Få tilgang til data

Evnen til å skaffe seg tilgang til tilbudte data fra annen aktør. Omfatter evnen til å oppdage datakilder og sette opp funksjon (klient) for å ta i bruk datakilden. Videre må virksomheten beskrive hvordan den ønsker å integrere eksterne informasjon i intern dataflyt, inkludert hvordan interne fagsystem og mellomvare skal bruke, vise og lagre data fra eksterne. Det må etableres en klientfunksjon som tar i bruk api'et fra den eksterne datatilbyderen og denne må integreres med interne systemer. 

![Få tilgang til data](img/213877674.png)

### Finne relevante data

Evnen til å finne kilder for informasjon om en gitt pasient ~personer~ ~eller informasjonskategorier~.

![Få tilgang til data](img/213877716.png)

## Eksempel: Realisere slå opp og dele målinger

Behov knyttet til dele egne målinger og slå opp andres målinger kan realiseres med å implementere prosesser for å avgi egne data gjennom en Datadelingstjeneste og en prosess for å fastsette hvilke målinger og på hvilken måte disse skal struktureres, samt hvilke målinger som skal tilgjengeliggjøres gjennom datadelingstjenesten. Datadelingstjenesten må dokumenteres i form av API-dokumentasjon som kan benyttes av konsumenter som ønsker å få tilgang til data som er tilgjengelig for oppslag gjennom datadelingstjenesten.

![Realisere slå opp](img/217121564.png)