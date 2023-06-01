---
title: Anbefalte tiltak
---

| Status           | Version | Maturity | Normative level |
| :--------------- | :------ | :------- | :-------------- |
| <span style="background-color:BlueViolet">Prerelease</span> | v0.9.0 | review | ikke normert |

Denne delen av målarkitekturen skal foreslå tiltak som kan gjennomføres for å understøtte etableringen av datadeling mellom virksomheter innen for behovsområdet DHO.

## Prioritert liste over anbefalte tiltak

Listen nedenfor viser en prioritert liste over tiltak vi mener er nødvendig for å realisere datadeling som skal understøtte DHO-tjenester. For å oppnå effektiv spredning av datadeling innen DHO området mener vi tiltak 1-3 er absolutt nødvendige. Tiltakene 4-6 bør realiseres for å understøtte forventede behov innen DHO og datadeling. Tiltakene er nødvendige for å oppnå helhetlige datadelingsløsninger som understøtter sammenhengende DHO forløp på en effektiv måte.  

1. [Felles tillitsmodell for datadeling](#felles-tillitsmodell-for-datadeling)
2. [Etablere fellesløsninger for lagring og grensesnitt](#etablere-felleslsninger-for-lagring-og-grensesnitt)
3. [Felles semantisk rammeverk for datadeling og DHO](#felles-semantisk-rammeverk-for-datadeling-og-dho)
4. [Vurdere fellesløsninger for utstyrslogistikk](#vurdere-felleslsninger-for-utstyrslogistikk)
5. [Etablering av PIL for datadeling](#etablering-av-pil-for-datadeling)
6. [Rammeverk for hendelsesbasert samhandling](#rammeverk-for-hendelsesbasert-samhandling)

### Felles tillitsmodell for datadeling

!!! quote ""

    Helsesektorens tillitsrammeverk definerer spilleregler og løsninger som virksomhetene som skal samhandle må akseptere og ta i bruk, slik at virksomheten kan få tilgang til helseopplysninger digitalt på en sikker, lovlig og effektiv måte.

#### Status for etablering av felles tillitsmodell - januar 2023

Norm for informasjonssikkerhet ([Normen](https://www.ehelse.no/normen/normen-for-informasjonssikkerhet-og-personvern-i-helse-og-omsorgssektoren#5.2.2%20Autentisering)) stiller krav til benyttelse av sikker autentiseringsløsning ved tilgang til helseopplysninger mellom virksomheter. Det gjennomføres arbeid knyttet til å etablere felles tillitsmodell i forbindelse med utbredelse av dokumentdeling i regi av program digital samhandling. Norsk Helsenett etablerer fellestjenester for felles tillitsmodell og løsningen skal prøves ut og videreutvikles i forbindelse med Dokumentdeling gjennom kjernejournal.

#### Anbefalt tiltak

I tillegg til dokumentdeling gjennom kjernejournal er digital hjemmeoppfølging og deling av målinger identifisert som utprøvingskandidat for felles tillitsmodell. Utprøving av felles tillitsmodell for datadelingstjenester i tillegg til dokumentdeling vil kunne gi viktig tilleggskunnskap sett fra helsetjenesten som prøver ut DHO sitt perspektiv. Vi vet foreløpig lite om kravene som stilles til tillitsmodellen knyttet til datadeling. Hypotesen er at tillitsmodellen for datadeling og dokumentdeling fungere likt, er det viktig å få bekreftet den antakelsen ved å prøve ut tillitsmodellen også for datadelingsløsninger.

Det anbefales at virksomheter som etablerer datadeling mellom virksomheter tar i bruk felles tillitsmodell og fellskomponenter som felles tillitsanker.  

### Etablere fellesløsninger for lagring og grensesnitt

Konseptet for [distribuerte datadelingsløsninger i sentral infrastruktur](Konsepter-realisering.md#distribuerte-datadelingslsninger-i-sentral-infrastruktur) er basert på at grensenitt og lagring av helsedata etableres i sentral infrastruktur, for eksempel hos NHN. De sentrale konseptene baserer seg også på etablering av lagring og grensesnitt sentralt. Velferdsteknologisk knutepunkt (VKP) som er en tjeneste hos NHN tilbyr formidling av journalverdige opplysninger mellom systemer som ellers ikke snakker sammen. Det jobbes med å etablere felles løsning for lagring og avgivelse av data som ny funksjon i VKP som vil kunne benyttes av utprøving- og spredningsprosjekter for DHO som gjennomføres i dag.  

Det er flere problemstillinger må håndteres når det gjelder bruk av VKP for å tilby denne typen løsninger.

* Merkantile forhold knyttet til konkurransehensyn og betaling for tjenester i VKP.
* Avtalerammeverk for å benytte funksjonalitet for datadeling som etableres sentralt.
* Det eksisterer juridiske problemstillinger knyttet til sammenstilling av DHO målinger på tvers av virksomheter i et sentralt datalager, siden dette ikke kan gjøres innenfor gjeldende rett.
* Styring, forvaltning og nyttevurderinger knyttet til sentral løsning, hvordan prioriterer man mellom identifiserte behov.

#### Anbefalte tiltak

Det må utredes hvordan alle punktene over skal løses hvis det etableres sentral infrastruktur for datadeling knyttet til DHO. Utredning må peke på hvordan etablering og forvaltning av fellesløsninger skal fungere i relasjon til merkantile, juridiske og styringsmessige forhold.

### Felles semantisk rammeverk for datadeling og DHO

Kapitelet som beskriver [konsepter for realisering](Konsepter-realisering.md) av datadeling mellom virksomheter og omsorgsnivå peker på nødvendigheten av felles semantiske spesifikasjoner for å understøtte distribuerte konsepter og [semantisk samhandling](Semantisk-samhandling.md). Det er behov for semantiske spesifikasjoner ved etablering av sentrale/nasjonale løsninger også, men dette vil realiseres gjennom grensesnittspesifikasjonene i den sentrale løsningen.  

Utprøving og spredningsprosjektene som gjennomføres nå baserer seg på et lite sett [HL7 FHIR](https://hl7.org/fhir/) profiler som beskriver det semantiske innholdet i [målinger](https://simplifier.net/guide/VelferdsteknologiskknutepunktDHOR4/Observation?version=current) som kan utveksles mellom virksomhetene. Profilene beskriver i hovedsak tre forhold knyttet til utveksling av informasjon mellom virksomhetene:

* Overordnet brukertilfelle profilene understøtter.
* Hvilken informasjon som er minimum for at informasjonen skal være nyttig.
* Regler for informasjonsinnhold i de spesifikke informasjonselementene.
  * Inkluderer regler om bruk av felles terminologi og kodeverk.

Vi tror det er nødvendig at det eksisterer felles beskrivelse av dette på tvers av virksomheter for at datadeling skal fungere på en god måte, dette er uavhengig av om distribusjonen av data baserer seg på en sentral eller distribuert modell. Ved en distribuert modell er det imidlertid et ufravikelig krav at det er felles regler for hvordan informasjonen struktureres ved digital samhandling, ellers vil etablering av oppslagstjenester mot mange ulike grensesnitt bli en uoverkommelig oppgave hvor utviklerne må forholde seg til en rekke typer semantiske spesifikasjoner. Integrasjon mot bakenforliggende systemer vil også bli svært komplisert.

#### Utestående arbeid knyttet til utveksling av målinger

På nåværende tidspunkt er det bare et fåtall profiler som er utviklet, disse har også sett lite praktisk bruk og er implementert i få løsninger. Det er viktig at profilene videreutvikles i tre retninger:

* Kvantitet - det er få brukertilfeller som er dekket av eksisterende profiler, det må testes og utvikles flere for å dekke flere brukertilfeller og flere typer informasjonstjenester.
* Kvalitet - profilene må implementeres i flere løsninger og testes i praktisk bruk for å kvalitetsikre at innholdet er tilstrekkelig for praktisk klinisk bruk og bekrefte at integrasjon mot flere ulike løsninger kan gjennomføres.
* Innhold - dagens profiler beskriver informasjonsinnholdet, men også lovlige søkeparametere bør detaljeres i neste versjon av profilene. På denne måten kan man sikre at datadelingstjenestene tilbyr lik søkefunksjonaliteten uavhengig av hvem som implementerer grensesnittene.

#### Andre informasjonsbehov

På nåværende tidspunkt eksisterer det bare profiler for å utveksle målinger mellom virksomheter. Det er også behov for å understøtte utveksling av annen informasjon på en standardisert måte ved hjelp av datadeling og API. Forløpig er spesielt to typer informasjon prioritert:

* Behandlings- og egenbehandlingsplan - Prosjektet som utvikler den sentrale løsningen for behandling og egenbehandlingsplan har også utviklet en spesifikasjon for utveksling av planer og FHIR profiler for dette. Disse profilene bør samordnes med behovene som eksisterer i andre planverktøy som er tatt i bruk i helsesektoren.
* Tjenester inkludert hjelpemidler og logistikk - hvis det igangsettes arbeid knyttet til fellesløsninger eller utviklingen av en distribuert modell for å håndtere dette området som er beskrevet i [tiltaket](#vurdere-felleslsninger-for-utstyrslogistikk)

#### Anbefalte tiltak

Det anbefales tiltak knyttet til alle de tre retningene som beskrives i forrige avsnitt, tiltak for å øke kvantiteten av profiler for å dekke flere brukertilfeller og tiltak for å øke kvaliteten ved å teste eksisterende profiler bedre, er de tiltakene som haster mest.

### Vurdere fellesløsninger for utstyrslogistikk <!--Hva er det viktige å få frem i dette avsnittet? Hvordan en kan svare ut kjente utfordringer som krav til utstyrets evne til å dele informasjon og logistikk rundt utstyr? Vurdere en annen overskrift for å vise til dokumenterte barrierer: eks. Vurdere felles anskaffelse og forvaltning av tekniske løsninger/system-->

Innspill fra aktørene som arbeider med spredning og utprøving av DHO har pekt på to store utfordringer knyttet til etablering av DHO tjenester. Det ene handler om samhandling som behandles i dette dokumentet. Et annet behov som er identifisert er knyttet til tildeling og forvaltning av det tekniske utstyret som skal samle målinger hjemme hos pasienten, ofte omtalt som DHO-system.

Det er identifisert mange behov knyttet til administrasjon av utstyr og bare noen av disse kan dekkes med ren oversikt over hvilket utstyr pasienten har, uavhengig av hvem som har tildelt dette:

* Kjenne til tjenester, ytelser og hjelpemidler og hvilke aktører som har tildelt disse.
* Kjenne til om relevant utstyr er tildelt fra andre aktører.
* Unngå dobbelt sett av utstyr med overlappende funksjonalitet.
* Tilgang til data fra utstyr.
* Tilgang til administrasjon av utstyr.

#### Anbefalt tiltak

Det anbefales at det settes igang arbeid som gjør det mulig for flere virksomheter å høste informasjon fra det samme utstyret, uavhengig av hvem som har tildelt utstyret. Det må først gjøres et mer grundig behovsarbeid og det må sannsynliggjøres at en slik løsning gir tilstrekkelig verdi til at det er formålstjenlig å etablere felles infrastruktur for å ivareta behovet.

### Etablering av PIL for datadeling

[Målarkitektur for datadeling i helse og omsorgssektoren](https://www.ehelse.no/standardisering/standarder/malarkitektur-for-datadeling-i-helse-og-omsorgssektoren) peker på nødvendigheten av å etablere pasientinformasjonslokalisator for å understøtte datadeling basert på distribuert lagring og etablering av grensesnitt for å avgi data. [Målarkitektur for datadeling i helse og omsorgssektoren](https://www.ehelse.no/standardisering/standarder/malarkitektur-for-datadeling-i-helse-og-omsorgssektoren) slår videre fast at det ikke eksisterer noen rettslig hjemmel for å etablere en nasjonal tjeneste som sammenstiller informasjon om hvilke API-tjenester som har informasjon en bestem pasient på nasjonalt nivå.

!!! quote "Pasientinformasjonslokalisator"

    Det er i en rekke situasjoner tilknyttet datadeling behov for å kunne fremskaffe en oversikt over hvem som har en pasientjournal for en gitt pasient. 
    ...
    Et slikt register bør etableres som en felleskomponent hvor det fremgår hvem som har helseopplysninger om en gitt pasient. Vi har valgt å kalle denne felleskomponenten for pasientinformasjonslokalisator, forkortet til PIL.

#### Status for etablering av PIL - juni 2023

Det eksisterer i dag ikke noen tiltak knyttet til å etablere felleskomponent eller fellestjeneste for PIL i samhandlingsinfrastrukturen for helsesektoren

#### Anbefalt tiltak

Spredning av DHO og understøtte behov for datadeling på tvers av mange virksomheter innenfor en region er avhengig av en regional, eller nasjonal tjenste for metadataformidling. Spesifikt gjelder dette informasjon om hvilke datadelingstjenester som har informasjon om en bestemt pasient. Det er uavklart hvor stort behovet er, siden det på nåværende tidspunkt ikke finnes noen oversikt over hvor mange datadelingsløsninger virksomhetene vil etablerer. Det mangler også utredning knyttet til konsept og juridiske avklaringer knyttet til etablering av PIL som en fellestjeneste i samhandlingsinfrastrukturen. Det er derfor behov for å:

* beskrive behovet basert på etableringen av datadelingsløsninger for deling av data mellom virksomheter.
* utarbeide et konsept for PIL som innenfor gjeldende rett, basert på desentralisert modell.
* alternativt utarbeide forskrift som regulerer behandlingsgrunnlaget for PIL informasjon i en sentralisert løsning.
* planlegge arbeidet med etablering og innføring av PIL.
* etablere PIL som en fellestjeneste i samhandlingsinfrastrukturen for helsesektoren.
<!-- Litt usikker på om det skal være stor eller liten forbokstav i denne punktlisten. -->

### Rammeverk for hendelsesbasert samhandling

Gjennom behovsarbeidet er det avdekket flere informasjonstjenester som bør understøttes med hendelsesbasert arkitektur. Dette er dokumentert i oversikten over informasjonstjenester. Noe av behovet knyttet til hendelsesbasert arkitektur er knyttet til sanntidsoppdateringer av informasjon som andre virksomheter samler inn eller dokumenterer om en pasient, dette er spesielt viktig i enkelte tjenesteforløp hvor DHO benyttes. Også informasjon fra utstyr som andre virksomheter plasserer ut hos pasient kan det være avgjørende å få sanntidsoppdateringer fra.  

Hendelsesbasert samhandling er i bruk i mange andre sektorer, spesielt knyttet til oppdateringer av felles datakilder. Det moderniserte folkeregisteret tilbyr for eksempel hendelser til konsumentene slik at eksterne virksomheter kan være oppdatert på endringer i folkeregisteret i sanntid eller nær sanntid. I helsesektoren er bruken av hendelsesbasert kommunikasjon mellom virksomheter å annse som en svært umoden samhandlingsform. Det er behov for generelle rammer og råd knyttet til etablering av hendelsesbasert samhandling. Norsk Helsenett har beskrevet et strategisk målbilde som blant annet inneholder en stor satsing i retning hendelsesbasert kommunikasjon med virksomhetene i sektoren. Det er flere tiltak som må gjennomføres før hendelsesbasert kommunikasjon kan fungere som samhandlingsform mellom virksomhetene i helsesektoren.

#### Anbefalte tiltak

* Kartlegging av eksisterende hendelsesbaserte løsninger og erfaringer fra arbeidet med disse.
* Kartlegging av virksomhetenes planer for å ta i bruk hendeslesbasert kommunikasjon.
* Enighet om felles målbilde knyttet til hvordan hendelsesbasert kommunikasjon kan benyttes og hvilke behov som dekkes best med hendelsesbasert kommunikasjon.
* Beskrive relevante fellestjenester i samhandlingsinfrastrukturen som må til for å understøtte hendelsesbasert kommunikasjon, det bør også etableres et veikart for når fellestjenestene kan etableres.