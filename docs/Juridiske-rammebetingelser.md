---
title: Juridiske rammebetingelser
---

| Status           | Version | Maturity | Normative level |
| :--------------- | :------ | :------- | :-------------- |
| <span style="background-color:gold">Work in progress</span> | v0.3 | draft | ikke normert |

## Innledning

Digital hjemmeoppfølging er underlagt det samme rettslige rammeverket som øvrig helsehjelp. Krav til behandling av helse- og personopplysninger som stilles i helselovgivningen og personvernregelverket må følges når en benytter digital hjemmeoppfølging som en integrert del av et behandlingsforløp. Ved bruk av digital hjemmeoppfølging må det dermed gjøres konkrete vurderinger i de enkelte tilfellene slik at det sikres at bestemmelsene om f.eks. dokumentasjonsplikt, tilgjengeliggjøring av opplysninger, taushetsplikt, ansvarsforhold, behandlingsgrunnlag, informasjonssikkerhet mv. oppfylles på vanlig måte.

Slik digital hjemmeoppfølging benyttes internt i en virksomhet i dag er det ikke nødvendig med regelverksutvikling. Det er først og fremst når virksomhetene har behov for å utveksle helseopplysninger på tvers av behandlingsnivåer (mellom primær- og spesialisthelsetjenesten), at det juridiske handlingsrommet blir utfordret. I dag benyttes hovedsaklig meldingsutveksling for å understøtte samhandling på tvers av virksomheter og omsorgsnivå, men i mange tjenesteforløp hvor DHO benyttes er det behov for samhandling som meldingsutvekslingen ikke kan løse. I disse tilfellene løses samhandlingsbehovet mellom virksomheter i en del tilfeller ved at å gi tilgang til det interne systemet i andre virksomheter ved å opprette en bruker hvor ansattforhold er satt til 0%. Dette gir tilgang til systemene, men er ikke en bærekraftig (eller lovlig) løsning. Det er derfor planlagt å prøve ut datadeling på tvers av virksomhetene for å oppnå en bedre informasjonsflyt og mer effektiv arbeidshverdag med utveksling av data til den andre virksomhetens systemer. Dette forutsetter at det i gjennomføringen av tiltaket særlig gjøres konkrete vurderinger knyttet til sikker tilgangsstyring.

Velferdsteknologisk knutepunkt (VKP) som driftes av Norsk helsenett (NHN), har i dagens VKP ingen lagring av data i løsningen. De innsamlede data ligger i ulike DHO-systemer/medisinsk utstyr og i lokal journalløsning. Det kan i utprøvingen og videre bli aktuelt å delvis lagre data fra digital hjemmeoppfølging hos dataansvarlig som en datadelingstjeneste eller sammenstilt sentralt på tvers av aktører. Det er foreløpig uavklart om et internt lager for datadelingstjeneste hos dataansvarlig er innenfor dagens regelverk. En nasjonal lagring av sammenstilte data (hvor en nasjonal aktør har dataansvar) vil etter vår vurdering kreve et annet juridisk grunnlag enn det som finnes i dag, og forutsetter derfor regelverksutvikling/forskriftsendring. Hvorvidt data skal lagres sentralt eller distribuert er foreløpig ikke avklart og må vurderes nærmere som del av utprøvingene som gjennomføres.

## Datadeling og DHO

![Datadeling i DHO](img/datadeling-dho.png)

Behovskartlegging har avdekket at det er behov for større bruk av datadeling (tjenester med funksjonalitet for oppslag) for å støtte informasjonsbehovene innen DHO. Dagens samhandlingsløsninger baserer seg i hovedsak på melding og dokumentutveksling, mens bruk av datadelingstjenester (basert på oppslag) mellom virksomheter er lite utbredt i helsesektoren. De datadelingstjenestene som eksisterer i helse er i stor grad sentraliserte tjenester knyttet til resept, kjernejounal og grunndata. De sentraliserte tjenestene som inneholder personlig helseinformasjon er særregulert i pasientjournalloven og har egne forskrifter som definerer omfanget og formålet med tjenesten. [lenketekst](https://lenken)

## Problemstillinger som er vurdert

Ettersom datadeling mellom virksomheter er lite brukt i helse- og omsorgssektoren, er også det juridiske handlingsrommet i noen grad uavklart for denne typen samhandling og samhandlingstjenestene som skal understøtte dette. I mars 2021 publiserte Direktoratet for e-helse en målarkitektur for datadeling i helse- og omsorgssektoren. Målarkitekturen for datadeling omhandler i hovedsak hvordan datadelingstjenester kan etableres med tilstrekkelig grad av sikkerhet og personvern som er pålagt de dataansvarlige. Vi har derfor ikke sett det som nødvendig å vurdere dette igjen i forbindelse med DHO. Målarkitekturen for datadeling beskriver hvordan dataansvaret er fordelt mellom virksomheter som benytter datadeling for samhandling. Ved overføring av informasjon ved hjelp av datadeling fungerer dataansvaret som ved andre samhandlingsformer, det vil si at mottakeren har dataansvar for sin behandling av mottatt informasjon.

Vi har særlig vurdert følgende spørsmål som påvirker hvilke konsepter og løsningsvalg som kan vurderes:

1. Hvilke rammer setter regelverket for å etablere datadelingsløsninger sentralisert (i sentral infrastruktur), regionalt eller distribuert (i virksomhetenes egen infrastruktur)?
2. Hvilket handlingsrom har dataansvarlig i forhold til å etablere teknisk infrastruktur for datadeling.
   * Avklarer hvorvidt datadelingsløsninger kan etableres for en dataansvarlig av en tredjepart, der behandling av helseopplysninger er regulert av en databehandleravtale, eller om virksomheten er bundet til å håndtere alle funksjoner knyttet til datadeling innenfor egen infrastruktur og med en teknisk komponent for å lagre helseopplysningene.
3. Målarkitekturen for datadeling forutsetter at det opprettes en sentral komponent for å lokalisere data om en pasient kalt Pasientinformasjonslokalisator (PIL) for at datadeling mellom mange datadelingsløsninger skal fungere. Det er i dag ikke rettslig grunnlag for å etablere en PIL-komponent med sentral sammenstilling av informasjon, dette krever forskriftsendring. Regional PIL-komponenent kan etableres innenfor gjeldende rett (?).


### Nasjonal sentral datadelingsløsning med lagring

![Nasjonal sentral datadelingsløsning](img/sentral-kopi.png)

### Juridisk
Med dagens regelverk kan det ikke opprettes et eget nasjonalt behandlingsrettet helseregister uten at det gis egen forskrift for dette hjemlet i pasientjournalloven §10, eller at det etableres selvstendig hjemmelsbestemmelse for et nytt register i pasientjournalloven.
Informasjonen som eventuelt skulle lagres i det nasjonale registeret er heller ikke sammenfallende med innholdet i eksisterende nasjonale løsninger, som f.eks kjernejournal eller e-resept. Det er derfor ikke mulig å benytte noen av disse reglene for disse løsningene som grunnlag for et nasjonalt register for datadeling innen DHO. 

### Regionale datadelingsløsninger med lagring

![Regionale datadelingsløsninger](img/regional-datadeling.png)

### Juridisk
Ettersom dette konseptet forutsetter at også de lokale registrene videreføres, kan ikke et §9-samarbeid benyttes for å hjemle et felles sentralisert register  med hovedformål å tilgjengeliggjøre informasjon mellom virksomhetene i det regionale samarbeidet.


### Regionale fellesløsninger

![Regionale fellesløsninger](img/regional-felles-fokus.png)

### Juridisk
Et § 9-samarbeid kan benyttes for å etablere et felles behandlingsrettet helseregister for virksomhetene i samarbeidet . Registeret må komme til erstatning for de lokale §8-registrene. Intern tilgang/tilgjengeliggjøring etter pasientjournalloven § 19 må vurderes på vanlig måte. Her innebærer det ordinær tilgangsstyring til «egen» journal, ikke datadeling på tvers av nivåer/aktører.
o	Hvordan blir det mht kommunikasjon utover fellesløsningen?
-	Blir det som Distribuerte datadelingsløsninger (i virksomhetens infrastruktur), men slik at fellesløsningen her er 1 aktør?
o	Hva med PIL?


### Distribuerte datadelingsløsninger (i virksomhetenes infrastruktur)

![Distribuerte datadelingsløsninger (i virksomhetenes infrastruktur)](img/distribuert.png)

### Juridisk
Virksomhetene kan selv etablere datadelingsløsninger for tilgjengeliggjøring av pasientinformasjon fra egne interne systemer til klinikere  i andre virksomheter som har tjenstlig behov for informasjonen. Forutsetningen er at dette kan skje innenfor rammen av pasientjournalloven § 19, slik at hensynet til taushetsplikt, personvern og informasjonssikkerhet ivaretas. 
Det er usikkert hvordan PIL kan/skal etableres. Pasientjournalloven § 10 åpner for å gi forskrift om sentraliserte  infrastrukturkomponenter for å støtte samhandlingen. Bestemmelsen i seg selv er ikke tilstrekkelig.


### Distribuerte datadelingsløsninger (i sentral infrastruktur) (uavklart)

![Distribuerte datadelingsløsninger (i sentral infrastruktur)](img/distribuert-sentral.png)

### Juridisk
Virksomhetene kan velge å benytte en tredjepart  (databehandler) som tilbyr datadelingsløsning i stedet for å etablere dette selv. Forutsetningen er som over at dette kan skje innenfor rammen av pasientjournalloven § 19, slik at hensynet til taushetsplikt, personvern og informasjonssikkerhet ivaretas. 
Videre er det er en juridisk forutsetning at informasjonen fra hver virksomhet ikke sammenstilles med informasjon fra andre virksomheter i den sentrale infrastrukturen (hos databehandler), men at løsningene for lagring og grensesnittene etableres som logisk adskilte løsninger for hver virksomhet. Behandlingen av helseopplysninger i sentral infrastruktur må reguleres av en databehandleravtale mellom den enkelte virksomheten og leverandøren av infrastrukturen.
Som for en ren distribuert modell er det tilsvarende usikkerhet knytte til hvordan PIL kan/skal etableres.


