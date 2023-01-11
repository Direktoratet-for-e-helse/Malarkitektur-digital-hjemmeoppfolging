---
layout: default
title: Overordnet behovsbilde for samhandling DHO
nav_order: 5
---

| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
|<span style="background-color:gold">Work in progress</span> | v0.8 | review  | ikke normert |

Helse- og omsorgssektoren har behov for mer effektiv samhandling for å øke tilgjengeligheten til relevante helseopplysninger. Målbildet for helhetlig samhandling er å tilby informasjonstjenester på en samhandlingsinfrastruktur som representerer et sett av informasjonsbehov som ikke er tilstrekkelig dekket i dagens nasjonale e-helseløsninger for samhandling. Hver informasjonstjeneste gir mulighet for å utveksle eller dele helseinformasjon mellom ulike aktører. Særskilte behov løses nasjonalt når det gir vesentlig gevinst/ nytte. Høy semantisk samhandlingsevne (hva dataene betyr og hvordan de er definert) er nødvendig for å lykkes med dette.Arbeidet med behov for informasjonsdeling i behandlingsforløp der digital hjemmeoppfølging tilbys sees i sammenheng med målbildet for helhetlig samhandling. Kartlegging av behov for deling av informasjon, fra innbygger til helsepersonells løsninger, er utført med ulike perspektiv.  

Behovene i helsetjenesten ligger til grunn for etablering av samhandlingsløsningene i sektoren og legger premissene for hvilke samhandlingsløsninger som skal etableres og videreutvikles. Behovene knyttet til tjenesteforløp der helsehjelp ytes til pasienter som mottar digital hjemmeoppfølging (DHO) er i stor grad overlappende med andre tjenesteforløp. Vi kan derfor lære mye om nødvendige samhandlingsløsninger i sektoren ved å se spesielt på sammensatte tjenesteforløp innen DHO. Behovene henter vi fra utprøvingsprosjekter og tjenesteeiere i helse- og omsorgssektoren. Erfaring fra utprøvingsprosjektene skal over tid føre til mer spesifikk behovskartlegging knyttet til erfaring med utveksling av informasjon mellom virksomheter og behandlingsnivå (primær- og spesialisthelsetjenesten) knyttet til DHO. Vi skiller i det videre arbeidet mellom informasjonsbehov og funksjonelle krav.

**Merk:** Målarkitekturen tar høyde for å gi et overordnet behovsbilde for hele DHO-området beskrevet over.  

## Overordnede brukerhistorier 

Målbilde for samhandling begrenser seg til å understøtte ytelse av helse- og omsorgshjelp. Dette inkluderer å sikre kontinuitet i direkte helsehjelp, for eksempel når pasienter skrives ut fra sykehus og beveger seg mellom omsorgsnivå og det er behov for oppfølging i kommunen der tjenesten digital hjemmeoppfølging kan benyttes. Samhandling bidrar til økt pasientsikkerhet og kvalitet gjennom å legge til rette for deling av korrekt informasjon for heslsepersonell med tjenstlig behov. Formen som er valgt for funksjonalitetsbeskrivelse er brukerhistorie. En kortfattet beskrivelse av hvem som har behov, hva slags funksjonalitet det er behov for og hvorfor funksjonaliteten gir verdi.

Samhandlingstjenester i behandlingsforløp der tjenesten digital hjemmeoppfølging benyttes skal tilrettelegge for følgende funksjonelle behov:
 <!--Forslag til ny beskrivelse av funksjonelle behov (nummerert) for å ikke ta bort de tidligere beskrivelsene-->
1. Som helsepersonell har jeg behov for tilgang til oppdatert informasjon som er nødvendig for å yte helsehjelp til pasient på en effektiv måte
1. Som helsepersonell har jeg behov for å slippe å registrere samme informasjon flere ganger i ulike system, for å spare tid og unngå feil ved duplisering av informasjon
1. Som helsepersonell har jeg behov for å samarbeid med pasient og annet helsepersonell om utarbeidelse og oppfølging av behandlings- og egenbehandlingsplaner, slik at oppdaterte planer er tilgjengelig for alle aktører og for å unngå forsinkelser i oppfølging av pasient
1. Som pasient har jeg behov for tilgang til oppdatert og relevant informasjon for å mestre og ivareta egen helse
1. Som pasient har jeg behov for at helsepersonell med tjenstlig behov har tilgang til relevant informasjon uavhengig av hvem som har registrert informasjonen, slik at jeg slipper å gjenfortelle historien min

![Samhandlingsbehov](https://user-images.githubusercontent.com/6229665/201673221-debad9fc-b32f-42fb-b0d4-0c8dbeefc2ab.png)

## Tjenesteforløp og samhandling

Som en ramme for behovskartlegging beskrives generelle prosesstrinn som de fleste tjenesteforløp gjennomgår. Et tjenesteforløp beskriver organisering og oppgaver knyttet til å yte helsetjenester til pasienter som følges med digital hjemmeoppfølging. Prosesstrinnene er angitt på overordnet nivå og har som formål å knytte samhandlingsbehovene til et <!--Er det her ment å knytte til et behandlingsforløp eller tjenesteforløp? Hele denne innledende teksten må endres når vi er enige om begrepsbruk og innholdet-->generelt tjenesteforløp/pasientforløp. De overordnede prosesstrinnene kan spesifiseres ved behov for å synliggjøre hvordan samhandlingen understøtter mer spesifikke tjenesteforløp. Ved analyse av samhandlingsbehovene konsentrerer vi oss om hvordan tjenesteforløpet kan understøttes med nye eller endrede samhandlingsløsninger og det meste av arbeidet vil derfor handle om prosessene for **samhandling**. Vi tar utgangspunkt i en generell prosess for tjenesteforløpet i helsetjenesten (for eksempel knyttet til DHO) i figuren under.

![Prosess for tjenesteforløp og samhandling](img/tjenesteforlop-og-samhandling.png)

I tillegg til behovskartlegging knyttet til [utprøvings- og sprednings-prosjekter](Bakgrunn-behov.md) er den generelle beskrivelsen av  tjenesteforløpet basert på Helsedirektoratets anbefalinger knyttet til [Utvikling av helhetlige tjenesteforløp](https://www.helsedirektoratet.no/rapporter/digital-hjemmeoppfolging-sluttrapport-fra-nasjonal-utproving-2018-2021/utvikling-av-helhetlige-tjenesteforlop).

* **Søknad/Henvisning** er prosesser knyttet til å motta søknad eller henvisning fra andre deler av helsetjenesten  eller innbygger/pårørende. Eksempler kan være at en pasient er tildelt en tjeneste basert på søknad som omfatter hjemmetjenester kombinert med utplassering av DHO-utstyr/ medisinsk utstyr i pasientens hjem
* **Oppstart** er oppstart av ny helsehjelp basert på søknad/henvisning med bakgrunn i behov og/eller diagnose, pasientens symptomer med utredning av pasientens tilstand. Oppstart inkluderer planlegging av behandling/oppfølging og tiltak som skal gjennomføres, og opplæring av involvert helsepersonell og pasienter/pårørende, for eksempel knyttet til bruk av medisindispenser eller annet DHO utstyr/ medisinsk utstyr og utarbeidelse av plan.
* **Behandling og oppfølging** av pasient er det mest sentrale prosessteget i tjenesteforløpet og vil omfatte alle former for vurdering, rapportering, oppfølging og behandling som gjennomføres. Det kan være oppfølging ved hjelp av teknologi, hjemmebesøk eller behandling som krever besøk/innleggelse på helseinstitusjon
* **Evaluering** innebærer å gjennomgå hvordan oppfølgingen fungerer, vurdere nye tiltak og eventuelt justere eksisterende tiltak.
* **Avslutte** tjeneste innebærer at tjenesteforløpet avsluttes etter evaluering.

Prosessen for **Samhandling** er brutt ned til generelle steg som kjennetegner en samhandlingsprosess, og kan understøttes på mange måter av automatiserte eller manuelle prosesser og funksjoner.

* **Innhente informasjon** er enhver prossess hvor en aktør leser, finner eller henter informasjon fra andre interne eller eksterne kilder
* **Vurdere og gjennomføre tiltak** er enhver prosess hvor informasjon benyttes til å vurdere og gjennomføre faktiske tiltak for en pasient
* **Produsere informasjon** er enhver prosess knyttet til å dokumentere tiltakene som er gjennomført og vurderingene som ligger til grunn for tiltakene
* **Dele informasjon** er enhver prosess knyttet til å dele eller tilgjengeliggjøre produsert informasjon, slik at andre aktører kan konsumere (bruke) informasjonen

## Kartlagte behov og funksjonelle krav

For å understøtte tjenesteforløp der pasienter følges med digital hjemmeoppfølging på en effektiv måte er det identifisert en rekke brukerbehov som kan understøttes med bedre samhandlingsløsninger. Dette kapitelet oppsummerer de mest sentrale behovene og funksjonelle krav som kan utledes fra disse.

### Hypotese knyttet til behov <!--Foreslår å flytte hypotesen til under tabellen slik at det er sammenheng i første avsnitt-->

Hypotesen beskriver en antagelse som er fremkommet gjennom behovskartleggingen knyttet til DHO. Det ligger i hypotesens natur at den bør testes før målarkitekturen ferdigstilles. Det er foreløpig et åpent spørsmål hvordan disse hypotesen testes og om den kan testes som en del av utprøvingsprosjektene innen DHO.

* Samhandlingsbehovet knyttet til tjenesteforløp med DHO integrert er størst regionalt
  * Arbeidet med målarkitektur for DHO fokuserer derfor på å tilrettelegge for samhandling på regionalt nivå
<!-- Hvordan unngår vi å ta arkitekturvalg som hindrer oss fleksibilitet senere -->

### Identifiserte behov

Tabellen under viser en oversikt over:

* Hvilken sluttbruker rolle som har behovet <!--sette innen parentes her med tekst: roller er beskrevet i kap....-->
* Hvilken prioritet og tidsperspektiv behovet har
  * Prioritet scores i kategoriene høy/middels/lav/ekstern ut fra antagelse om forventet nytte/effekt
    * Høy nytteverdi betyr at tilfredstillels av behovet vil gi stor nytte og det er mange brukere
    * Middels nytteverdi betyr at tilfredstillelse av behovet vil kunne føre til spart tid og bedre kvalitet men er ikke kritisk for å ta i bruk tjenesten <!--Her mener vi vel tjenesteforløpet? Tilby DHO uten at informasjonsdeling er på plass?-->
    * Lav nytteverdi angir behov hvor nytten for brukeren er liten eller at behovet innehas av få brukere
    * Ekstern betegner behov som må spilles inn til andre prosjekter og behovet må tilfredstilles (i hovedsak) av løsninger som ligger utenfor omfanget av målarkitekturen
  * Tidsperspektiv kategoriene angis med: Kort (0-1 år), mellom(lang) (1-3 år) og lang (3-5 år)
* Beskrivelse av behovet
* Viktige funksjonelle krav som må oppfylles for å tilfredstille behovet på en god måte

|Rolle| Prioritet / tidsperspektiv|Behov|Funksjonelle krav|
|-----|-----------|-----------------|--------------------|
|Helsepersonell (kommune, spesialist og fastlege)|høy / lang|Bedre støtte for eksplisitte ansvarsoverganger mellom virksomheter||
|Helsepersonell (kommune, spesialist og fastlege)|høy / mellom|Finne hvilken informasjon andre virksomheter og behandlingsnivåer har om pasienten|Søkefunksjonalitet for å finne hvilke virksomhetene som har informasjon om pasienten|
|Helsepersonell (kommune, spesialist og fastlege)|høy / kort|Vise informasjon som andre virksomheter og behandlingsnivåer har samlet inn om pasienten|Felles informasjonsstruktur og innhold er viktig både for: </br> - Å vise informasjon fra flere eksterne virksomheter </br> - Tilby enhetlig søkegrensesnitt på tvers av flere virksomheter </br> - Sammenstilling av informasjon fra flere kilder i felles visning|
|Helsepersonell (kommune, spesialist og fastlege) | høy / mellom | Vise trender og sammenhenger mellom informasjon samlet inn i egen og andre virksomheter|Felles informasjonsstruktur og innhold er viktig både for: </br> - Å vise informasjon fra flere eksterne virksomheter </br> - Tilby enhetlig søkegrensesnitt på tvers av flere virksomheter </br> - Sammenstilling av informasjon fra flere kilder i felles visning|
|Helsepersonell (kommune, spesialist og fastlege)|høy / kort|Samhandlingen og arbeidsflyten skal ikke medføre dobbeltarbeid|Det skal ikke være nødvendig å registrere samme informasjon flere ganger (i ulike systemer) eller logge seg på i ulike systemer for å gjennomføre arbeidsoppgaver knyttet til samme pasient og tiltak (SSO) /Er det noe krav til innlogging med tanke på HPR, må alle være registrert der? Trenger også personell som sekretærer tilgang?|
|Helsepersonell (kommune, spesialist og fastlege)|middels / mellom|Arbeidsflyt og samhandling må støttes i en enhetlig utformet brukerflate|Unngå særegne systemer for oppslag i DHO resultater </br> Unngå mange ulike utformede arbeidsflater som ikke er integrert|
|Helsepersonell (kommune, spesialist og fastlege)|middels / mellom|Det må være mulig å kvalitetssikre relevant informasjon ved å se hvor informasjonen kommer fra og hvordan den er samlet inn|Proveniens og metadata med riktig detaljnivå må følge informasjonen når den utveksles|
|Helsepersonell (kommune, spesialist og fastlege)|middels / mellom|Tilgang til ulike typer informasjon for å understøtte tjenesteforløpet knyttet til flere pasientgrupper.|Aktuelle pasientgrupper kan være KOLS syke, multisyke og andre pasientgrupper med behov for digital hjemmeoppfølging|
|Helsepersonell (kommune, spesialist og fastlege)|ekstern (høy) / mellom|Samarbeide om utarbeidelsen av behandlingsplan og egenbehandlingsplan med pasienten og klinikere fra andre virksomheter|Det må eksistere felles kilde til planer og felles verktøy for samarbeid om planer|
|Helsepersonell (kommune, spesialist og fastlege)|ekstern (høy) / lang|Det må være tydelig og avklart sammenheng mellom tiltak i egenbehandlingsplanen og DHO utstyr/verktøy benyttes i egenbehandlingsplanens tiltak|Det må være lett å se informasjon fra plan og DHO-utstyr i sammenheng|
|Helsepersonell (kommune, spesialist og fastlege)|høy / mellom|Behov for individuell tilpasset tjeneste ut fra type pasient og behov knyttet til daglig oppfølging||
|Helsepersonell (kommune, spesialist og fastlege)|høy / lang|Å være oppdatert|Når data i kilden endrer seg, skal løsningen oppdatere seg uten opphold. Dette skal også skje når dataene endrer seg hyppig.|
|Helsepersonell (kommune, spesialist og fastlege)|middels / lang|Tilgang til sanntidsinformasjon der det er relevant (målinger for eksempel)|Dette er ikke påpekt av tjenestene som er en del av utprøvingene, men er en del av HSØ sitt målbilde for utveksling av målinger|
|Helsepersonell (kommune, spesialist og fastlege)|middels / lang|Behov for å ivareta at utstyret følger pasienten uavhengig hvem som er behandlingsansvarlig|Løsninger knyttet til delt sanking av data og oppfølging av utplassert utstyr hos pasient stiller store krav til hvordan utstyrslogistikken samordnes mellom partene. Dette inkluderer utveksling av informasjon om utstyrstype, fastvareversjoner, strømstatus, feilmeldinger og direkte tilgang til automatisert og manuell teknisk inngripen med utstyret via internett eller på stedet. I og med at det ikke eksisterer gode standardiserte løsninger knyttet til utstyrslogistikk av heterogent utstyr anskaffet fra mange virksomheter har vi valgt å ikke inkludere utstyrslogistikk i det kortsiktige målbildet. Dette kan også påvirke muligheten til å ivareta denne delen av behovet på kort sikt.|
|Fastlege||Fastlegen har de samme behov som helsepersonell for øvrig, men har ikke daglig oppfølging av pasienten i en DHO tjeneste. De har behov for informasjon om pasient på forespørsel når pasienten tar kontakt, eller ved henvendelse fra annet helsepersonell.|Likt behov som for øvrig helsepersonell? Systemer: EPJ og noen bruker KJ og Helsenorge.|
|Pasient / pårørende|høy / kort|Som innbygger ønsker jeg tilgang til informasjon som gjør det mulig å forstå og mestre egen helse. Finne informasjon om pasienten </br> Vise informasjon som gjelder pasienten </br> Vise trender og sammenhenger mellom informasjon samlet inn av flere virksomheter. Det er behov for å ha dialog med helsepersonell og gi tilbakemelding til tjenesten på en enkel måte.|Det må være lett for pasient å få tilgang til egen helseinformasjon. </br> Pårørende må ha mulighet til å få innsyn og være deltakende ut fra behov og ønske fra pasient.|
|Pasient / pårørende|middels / kort|Avlevere data basert på mål og tiltak i oppsatt plan.|Det må være lett for pasient å oppdatere data om egen helse og behandling i en sammenhengende arbeidsflate|
|Pasient / pårørende|middels / kort|Det må være mulig for meg som pasient å se hvem som har tilgang til mine data for å ivareta mitt personvern.|Det må være lett for pasient å se hvem som har tilgang til mine data.|
|Pasient / pårørende|høy / mellom|Jeg må være sikker på at relevant helsepersonell får tilgang til tilstrekkelig informasjon slik at jeg kan motta best mulig helsetilbud og at helsetjenesten iverksetter de beste tiltakene for å ivareta min helse.|Pasient skal ikke trenge å videreformidle informasjon mellom helsepersonell, det skal skje ved hjelp av datadeling på tvers.|

## Roller i tjenesteforløp med digital hjemmeoppfølging <!--Kunne beskrivelsene av roller i pasientforløpet flyttes til bakgrunn - behov? Da kan vi fokusere på behov i dette kapittelet-->

Figuren viser en overordnet oversikt over roller som kan være involvert i DHO baserte tjenesteforløp. Denne rolleoversikten er basert på dialog med aktører fra kommune-, fastlege- og spesialisthelsetjenesten i to utprøvingsprosjekt, og vil derfor ikke være uttømmende.

[![Roller](img/roller.png)](img/roller.png)

| **Rolle** | **Definisjon** |
|---|---|
| Innbygger | Samlebetegnelse på alle roller en person kan ha som tjenestemotaker i helse- og omsorgssektoren enten som pasient, bruker eller pårørende |
| Pasient | Begrepet pasient brukes om personer som gis eller tilbys hjelp fra helsetjenesten eller som henvender seg til helsetjenesten med anmodning om helsehjelp (kilde Hdir) |
| Pårørende | Pårørende er en person som står en annen person særlig nær, for eksempel partner/ektefelle eller nærmeste familie. (Store Norske leksikon) |
| Nærmeste pårørende | Det er nærmeste pårørende som i enkelte tilfeller har en selvstendig rett til å motta informasjon, klage på vedtak mv. Det er altså ikke pårørende generelt, men den som oppgis som nærmeste pårørende, som har rettigheter og oppgaver etter helselovgivningen, og som helsepersonell har rettslige plikter overfor. (kilde Hdir) |
| Helsepersonell | En person som er nevnt i helsepersonelloven § 3 defineres som helsepersonell. For det første omfattes de som har autorisasjon eller lisens etter&nbsp;helsepersonelloven §§ 48&nbsp;og&nbsp;49.&nbsp;Dernest omfattes personell i helse- og omsorgstjenesten eller i apotek som yter helsehjelp, og studenter og elever som yter helsehjelp i forbindelse med helsefaglig opplæring. Medhjelpere til helsepersonell er helsepersonell når de får tildelt oppgaver fra helsepersonell. (kilde Hdir) |
| Helsepersonell fastlege | Samlebetegnelse for helsepersonell tilknyttet fastlegetjenesten. |
| Fastlege | Lege som inngår avtale med en kommune om deltakelse i fastlegeordningen, uavhengig av om legen er ansatt i kommunen eller er selvstendig næringsdrivende. (kilde: Lovdata) |
| Primærhelseteam <!--Ikke relevant hvis eksemplenme er LArvik, SIv - slik jeg leser figuren--> | Ivaretar daglig oppfølging av en pasient med DHO tjeneste på vegne av fastlegen (bare relevant i noen kommuner) |
| Helsestasjon for eldre |Drive forebyggende og helsefremmende arbeid, samt være et lavterskeltilbud med ansatte som har ulik helsefaglig bakgrunn og som jobber både i spesialist og primærhelsetjenesten|
| Helsepersonell kommune | Samlebetegnelse for helsepersonell tilknyttet kommunal helse- og omsorgstjeneste |
| Fysioterapeut | En fysioterapeut behandler og forebygger skader og sykdommer som gir smerte eller nedsatt funksjon i muskel- og skjelettsystemet (kilde utdanning.no) |
|Ergoterapeut |Arbeider helsefremmende og forebyggende for å fremme helse og aktivitet. Fokus på hva som hindrer eller muliggjør hverdagsaktiviteter og fokuserer på hva som er viktig i livet til den enkelte som skal hjelpes|
| Hjemmetjeneste |Helsetjenester som ytes hjemme hos pasient/bruker  |
| Farmasøyt |Arbeider med rådgivning knyttet til kunnskap om legemidler, hvordan de brukes og virker i kroppen. Sykehusfarmasøyt som bidrar med samstemming av legemidler/legemiddelliste |
| Oppfølgingsansvarlig | Den som har ansvar for den daglige oppfølging av pasient som mottar digital hjemmeoppfølging. Rollen ivaretas oftes av sykepleier som kan være ansatt henholdsvis i spesialist- eller kommunehelsetjenesten |
| Ambulant team |Et tverrfaglig team som følger opp multisyke eldre i overgangen mellom sykehus og hjem i et samarbeid mellom sykehus og kommune. Teamet gjennomfører kartleggingsarbeid for å se hvilke tilbud som kan være til hjelp for pasienten |
| Helsepersonell HF | Samlebetegnelse for helsepersonell tilknyttet spesialisthelsetjenesten. |
| Lege i spesialisthelsetjenesten|Lege ansatt på sykehus innen ulike fagområder|
| Helsesekretær |Tar imot henvendelser fra pasient/bruker og helsepersonell og utfører kontorfaglige oppgaver  |
| Eldrehelsekoordinator |Stilling som er del av tverrfaglig ambulant team  |

Referanser: [sentrale begreper definert i Program Digital Samhandling](https://sh.ehelse.no/akson/Dokumentbibliotek%20Forprosjekt%20Steg%202/20%20Leveranser/09.%20Sentralt%20styringsdokument/05%20Vedlegg%20SSD/Vedlegg%20A%20Sentrale%20begreper.docx?d=w5a50e9a879ab4c1a800b8a88cca9040c), Digdir, [Helsedirektoratet](https://www.helsedirektoratet.no/rundskriv/pasient-og-brukerrettighetsloven-med-kommentarer/alminnelige-bestemmelser/definisjoner#:~:text=pasient%3A%20en%20person%20som%20henvender,som%20p%C3%A5r%C3%B8rende%20og%20n%C3%A6rmeste%20p%C3%A5r%C3%B8rende.)

## Informasjonsbehov og informasjonstjenester

Ulike tjenesteforløp vil ha forskjellige behov for informasjon. Disse behovene beskriver vi i form av ulike typer informasjonsressurser og informasjonstjenester. Modellen viser hvilke overordnede informasjonsressurser og informasjonstjenester (gruppering av informasjonsbehov) det er avdekket behov for i forbindelse med DHO. Det er gjennomført en mapping av informasjonsressursene og hvordan informasjonsressursen henger sammen med informasjonstjenester definert i [Sentralt styringsdokument Akson - Helhetlig samhandling (bilag G2)](https://www.ehelse.no/publikasjoner/sentralt-styringsdokument-akson-helhetlig-samhandling-og-felles-kommunal-journallosning).

[![217121482](https://user-images.githubusercontent.com/6229665/201674228-84a1171d-0006-4720-a462-aaba5947dca8.png)](https://user-images.githubusercontent.com/6229665/201674228-84a1171d-0006-4720-a462-aaba5947dca8.png)

I tillegg er det identifisert behov for dialogtjenester for kommunikasjon mellom helsepersonell og mellom helsepersonell og innbygger:

![207618572](https://user-images.githubusercontent.com/6229665/201674334-dcbe578d-aeb3-40d1-9124-8ef0ce9087a1.png)

## Analyse av informasjonsbehov

Tabellen under viser en oversikt over identifiserte informasjonsbehov og kobling til tidligere identifiserte  informasjonstjenester fra bilag G2 Helhetlig samhandling. Tabellen oppsummerer:

* Informasjonsbehov
* Er informasjonsbehovet beskrevet i en informasjonstjeneste - informasjonsbehovene er mappet til informasjonstjenester definert for Helhetlig samhandling og felles kommunal journalløsning ([Bilag G2 definerer informasjonstjenestene](https://www.ehelse.no/publikasjoner/sentralt-styringsdokument-akson-helhetlig-samhandling-og-felles-kommunal-journallosning/Bilag%20G2%20Helhetlig%20samhandling.pdf))
* Hva betyr informasjonsbehovet
* Hvorfor er det behov for informasjonen
* Hvor kommer informasjonen fra (kilde)
* Hvordan blir informasjonen til
* Hvordan kan man samhandle om informasjonen for å dekke informasjonsbehovet
* Når er det behov for informasjonen og hvor lenge vil informasjon være relevant
* Er det sammenhenger/ avhengigheter med andre informasjonstjenester

| Informasjonsbehov | Informasjons-tjeneste | Hva | Hvorfor | Hvor (kilde) | Hvordan | Samhandlingsform | Når og hvor lenge | Sammenheng med andre informasjonstjenester |
|---|---|---|---|---|---|---|---|---|
| Målinger | Undersøkelser, målinger og funn (IT17) (Multimedia og MTU-målinger (IT07)) | Inneholder resultater fra målinger og registreringer av informasjon som beskriver pasientens tilstand.blodsukker, Pulsox, temperatur, vekt, blodtrykk og kroppsvekt. | Målinger av pasientens tilstand i øyeblikket, trender | pasienten, måleutstyr (Medisinsk Utstyr/DHO-system)DHO-system vil være hovedprodusent | Automatiske og manuelle registreringer | Slå opp og tilgjengeliggjøre </br> Sende og motta (internt i virksomheten) | Ved innleggelse og kontinuerlig oppfølging.Det kan være relevant ved behandlingsbeslutninger å ha tilgang til gamle målinger (flere år gamle) (Tilbakemelding fra lege spesialisthelsetjenesten) | IT08 Plan, IT23 Tjeneste, ytelser og hjelpemidler, IT09 Journaldokumenter og IT?? Vurderinger |
| Skjemabesvarelser | Undersøkelser, målinger og funn (IT17) | Innrapporterte data, eventuelt med poengsum,&nbsp; som beskriver pasientens tilstand.For eksempel skjemabesvarelser fra KOLS pasienter | Observasjon av pasientens tilstand i øyeblikket, trender | pasienten, Medisinsk Utstyr/DHO-system | Manuelle observasjoner | Slå opp og tilgjengeliggjøre |  |  |
| Journalnotat | Journaldokumenter (IT09) | Oppfølgingsnotater og sammenstillinger fra oppfølgingsansvarlig basert på innrapporterte data (målinger, varsel, skjemabesvarelser).Tidligere epikriser og sykepleiesammenfatninger, journalnotater, vurderinger, utredninger | Dokumentere hva som har skjedd, sammenstille informasjon for journalføringInnhente tilleggsinformasjon&nbsp; fra kommune/spesialist/fastlege? | Journalsystem/ DHO system som brukes i oppfølgingen/dokumentasjonsarbeidet | Manuelle føringer | Slå opp og tilgjengeliggjøre |  |  |
| Varsel | Undersøkelser, målinger og funn (IT17) | Basert på analyser/vurderinger av målinger eller skjemabesvarelserGrønne, gule, røde målinger – alvorlighetsgrad med referanseområde for normalverdi, Poengsum fra skjemabesvarelser, Ikke utførte oppgaver, inaktiv pasient | Varsle om målinger/poengsum utenfor referanseverdi eller manglende data, for å beslutte tiltak, eller som en del av journalnotatet.Eksisterer det samhandlingsbehov mellom virksomheter/internt i virksomheten rundt selve varslene til andre aktører?Det uttrykkes som et behov at dette kan deles til andre aktører (røde til spesialist etc). Men det er ikke konkretisert og løst p.t. kanskje et mer sentralt behov på sikt. | DHO-system, Medisinsk utstyr, analyseplattform | Manuelle eller automatiske vurderinger/analyser? | Ikke identifisert samhandlingsbehov utenfor virksomheten |  |  |
| Hendelse | Pågående og gjennomførte prosedyrer og behandlinger (IT19), Legemidler og vaksiner (IT03) | Noe som skjer med pasientenPåbegynt medisinkur, sykehusinnleggelse, undersøkelseVi har problemer med å definere "Hendelse" entydig, spesielt å skille det fra "Varsel". | Oversikt over behandlingsforløpet og statusEr det behov for å opprette nye hendelser og varsle andre aktører om dette? | Journalsystem/ DHO system både fastlege, spesialist og kommunehelsetjeneste. | Hovedsaklig manuell opprettelse av hendelser | Slå opp og tilgjengeliggjøre, hendelsesstrøm? endre og dele? |  |  |
| Legemiddelliste | Legemidler og vaksiner (IT03) | Oversikt over legemidler pasienten bruker |  |  |  |  |  |  |
| Pasientdemografi | Pasientdemografi (IT12) | Demografisk informasjon om pasientKontaktinformasjon, familierelasjoner, pårørendeinformasjon, vergeinformasjon eksisterer i FREG.Digitale kontaktpunkter, samtykkekompetanse, hjemmesituasjon, kontaktpersoner som ikke er familie eller verge (eksisterer ikke i folkeregisteret), (Kliniske bakgrunnsopplysninger (IT16)) | Oppslag i folkeregisterinformasjonEndre og dele utfyllende informasjon om pasienten demografiske opplysninger som ellers ikke finnes i personregisteret (hjemmesituasjon, utfyllende kontaktinformasjon etc.) | Journalsystem/ DHO system både fastlege, spesialist og kommunehelsetjeneste. | Automatiske oppslag og oppdateringer mot folkeregisteret.Manuelle tilleggsinformasjon og endring av disse. | Slå opp og tilgjengeliggjøre, hendelsesstrøm? endre og dele? |  |  |
| Tjenester, ytelser og hjelpemidler | Tjenester, ytelser og hjelpemidler (IT23) | Nåværende og tidligere kommunale og statlige tjenester og ytelser og hjelpemidler i bruk hos/av innbygger.Trygghetsalarm, medisindispenser, rullestol, hjemmehjelp, MTU-utstyr | Kjenne til tjenester, ytelser og hjelpemidler og hvilke aktører som har tildelt disse.Kjenne til om relevant utstyr er tildelt fra andre aktører. Unngå dobbelt sett av utstyr med overlappende funksjonalitet. | Journalsystem/ DHO system både fastlege, spesialist og kommunehelsetjeneste. | ? | Slå opp og tilgjengeliggjøreHendelsesstrøm for "egne" pasienter? |  |  |
| Skjemadefinisjon | Klinisk kunnskap (IT14) | Skjema (mal) for å registrere informasjon fra pasient?Forslag til betingede tiltaksplaner eller strukturerte regler til bruk i prosess- og beslutningsstøtte | Benyttes som grunnlag for pasientens egne registreringer, kunnskapsbaserte standardiserte spørsmål og målemetoder. (Denne kategorien var i en tidligere vurdering markert som irrelevant i forhold til Velferdsteknologi men gjennomgangen av behov basert på dialog med tjenesten tyder på at det er behov for denne typen klinisk kunnskap i forbindelse med DHO) | Standardiserte prosedyrer for behandling | ? | Slå opp og tilgjengeliggjøre |  |  |
| Plan definisjon |  | Retningslinje for behandling av en tilstand/diagnose/problem | Benyttes for å beskrive best-practice/guideline for behandling |  |  |  |  |  |
| Pasientplan | Plan (IT08) | Sykepleieplan og veiledende plan |  |  |  |  |  |  |
| Behandlingsplan (DBEP) | Plan (IT08) | Beskrivelser av forventet eller planlagt helsehjelp og andre tjenester for innbyggerBehandlingsplaner / tiltaksplaner inneholder blant annet planer og mål for utredning og behandling i regi av helsetjenesten, men også innbyggers bruk av egne ressurser | En behandlingsplan beskriver behandling for én eller flere problemstillinger. Dersom pasienten har flere&nbsp;problemstillinger/diagnoser, kan pasienten ha flere behandlingsplaner, eller det kan samordnes i en&nbsp;felles behandlingsplan. | Journalsystem/ DHO system både fastlege, spesialist og kommunehelsetjeneste. | En behandlingsplan kan opprettes i et pasientjournalsystem av den som til enhver tid er ansvarlig for en&nbsp;pasients behandling, eller annet helsepersonell som har et behandlende/terapeutisk forhold til&nbsp;pasienten&nbsp; | Endre og dele |  |  |
| Egenbehandlingsplan | Plan (IT08) | En plan med beskrivelse av tiltak som pasienten selv har&nbsp;ansvaret for å gjennomføreEgenmestringsplan – ta med rehabiliteringsplan, øvelser, tiltaksplan – alt pasienten skal gjøre selv samlet | Formålet med egenbehandlingsplanen er å oppdage forverringer&nbsp;tidlig, forebygge og å redusere utvikling av en forverring, hindre sykehusinnleggelse og gi økt&nbsp;trygghet og mestringsopplevelse. Egenbehandlingsplanen er en del av behandlingsplanen, og skal&nbsp;lagres i et pasientjournalsystem | Pasientens DHO system, Journalsystem/ DHO system både fastlege, spesialist og kommunehelsetjeneste. | En egnebehandlingsplan kan opprettes som en selvstendig egenbehandlingsplan eller i tilknytning til en&nbsp;eller flere behandlingsplaner. En pasient har kun én egenbehandlingsplan. | Endre og dele |  |  |
| Oppgaveruting |  | Hvem har ansvar for pasienten | Avklare hvem som tar ansvar for oppgaver |  | Henger sammen med hendelser og planer |  |  |  |
|  | Klinisk oppsummering (IT01) | Klinisk oppsummering er en informasjonstjeneste som vil tilby oppsummert og utvalgt informasjon som beskriver innbyggers behov for helsehjelp her og nå, og hvilken helsehjelp som mottas |  |  |  | Slå opp og tilgjengeliggjøre |  |  |
| Dialog | Tekstlig dialog (IT10) og Video (IT11) |  | Raske avklaringer mellom behandlingsnivåene |  |  | Slå opp og tilgjengeliggjøre </br> Sende og motta </br> I tillegg er det behov for synkrone samhandlingsformer med både tale, tekst og video |  |  |
| Vurderinger |  | Henger sammen med varsel og målinger, undersøkelser og funn |  |  |  |  |  |  |

## Informasjonstjenester som beskrives i DHO arbeidet

 Målarkitekturen skal beskrive behov for samhandling og informasjonstjenester som kan sikre at samhandlingen understøtter helsetjenesten på en hensiktsmessig måte. I arbeidet med å kartlegge informasjonsbehov skiller vi mellom informasjonsressurser og informasjonstjenester som må etableres for å understøtte informasjonsbehovet. I den grad det er nødvendig vil arbeidet også beskrive andre initiativer som etablerer informasjonstjenester () det er behov for i forbindelse med DHO og hvordan disse tjenestene bør tilgjengeliggjøres for å svare ut behov som er identifisert i forbindelse med DHO.  

 ! note "Samhandling på tvers"
    Gjennom dette arbeidet er det hovedfokus på hvordan data fra pasient (pasientregistrerte eller fra sensorer og utstyr) kan brukes på tvers av omsorgsnivå i helsetjenesten på en hensiktsmessig måte, og hvordan samhandlingen om denne informasjonen bør innrettes.

## Data fra pasient og informasjonstjenester

Hovedmålet for målarkitekturen DHO er å vise hvordan samhandlingen knyttet til data fra pasient skal gjennomføres, samtidig som den må vise hvilke andre informasjonstjenester som må være tilstede for å understøtte <!--tjenesteforløp - kun bruke dette hvis vi blir eninge om begrepsbruk--> en sammenhengende DHO tjeneste. Informasjonstjenestene som omfattes er i denne sammenhengen:

* Undersøkelser, målinger og funn (IT17 og IT07)
* Skjemabesvarelser og NEWS scoringer (IT17)
* Vurderinger og varsel basert på målinger (IT17)

! note "Pasientrapporterte data"
  Pasientene er aktive deltakere og bidragsytere i helsehjelpen de mottar og kan følges opp i hjemmet ved at pasientens egenmålinger, pasientrapporterte opplysninger om egen helsetilstand eller automatiske målinger, sendes digitalt til helsetjenesten.

## Informasjonstjenester i andre kategorier

Det er identifisert behov for samhandling om ytterligere informasjon og informasjonstjenester for å understøtte et  sammenhengende tjenesteforløp som inkluderer DHO. Dette inkluderer følgende behov:

* Plan (IT08)
* Hendelser (IT03 og IT19)
* Tjenester, inkludert hjelpemidler og logistikk (IT23)
* Legemiddelliste (IT03)
* Journalnotat (IT09)
* Klinisk oppsummering (IT01)
<!--Denner ikke med i tabell over behov og kobling mot informasjonstjenester i Akson. Vi får vurdere om det faktisk er IOT01 vi skal beskrive eller om det som er kommet frem dekkes av IT09 -->
<!-- SVAR: Denne er med i tabellen over og sammenhengene er vist i figuren https://user-images.githubusercontent.com/6229665/201674228-84a1171d-0006-4720-a462-aaba5947dca8.png-->
* Basisinformasjon pasient (IT12)
* Dialogtjenester (IT10 og IT11)
<!--Kunne denne vært koblet mot Kommunikasjon ved saksbehandling og Tekstlig dialog? Børd da beskrives i tabell-->
<!--SVAR vi behandler ikke dialog i detalj, men vi kan nevne IT10/IT11 og Tror ikke IT24 er relevant her-->

## Prioritering av informasjonstjenester

Her vises i prioritert rekkefølge de informasjonstjenestene som er mest etterspurt av helsepersonell:

1. Egenbehandlingsplan (IT08)
2. Legemiddelliste (IT03)
3. Målinger, vurderinger og varsel (IT17 og IT07)
4. Dialogtjenester (IT10 og IT11)

I tillegg er det en rekke andre informasjonstjenester som er høyt prioritert av tjenesten, disse vises i figuren: <!--Skulle vi vurdert å bruke figuren fra målbilde med alle informasjonstjenestene i arbeidet for å vise sammenhengene?-->
<!--SVAR: Nei, denne figuren har vist seg å fungere greit for å vise de høyest prioriterte informasjonsbehovene innen DHO-->
![226722458](https://user-images.githubusercontent.com/6229665/201674656-d97f3a8a-912a-41ee-b621-a1df9860d730.png)

Det utvikles samhandlingsløsninger knyttet til behov for [digitale behandlings- og egenbehandlingsplaner](https://www.helsedirektoratet.no/om-oss/forsoksordninger-og-prosjekter/digital-behandlings-og-egenbehandlingsplan) og [legemiddelliste](https://www.ehelse.no/prosjekt/program-pasientens-legemiddelliste) gjennom egne initiativ. Det er derfor besluttet at de viktigste tjenestene å utvikle samhandlingsløsninger for i DHO arbeidet nå som et første steg handler om Målinger, vurderinger og Varsel. Dette er informasjonstjenester som etterspørres fra mange virksomheter og alle omsorgsnivå i flere geografiske regioner.

## Detaljer om målinger
<!--Hva med vurderinger og varsel siden overskriften er målinger? -->
<!-- thomiz SVAR: Hva med vurderinger og varsel? Er det et spørsmål her? -->

Målinger består av flere typer måleparametere som beskriver pasientens helsetilstand og som kan bidra til å støtte oppfølging av behandling og synliggjøre endring i tilstand. Figuren viser omfanget for deling av målinger i første fase av utprøving av datadeling ved bruk av velferdsteknologisk knutepunkt (VKP):

![Datadeling av målinger med VKP](https://user-images.githubusercontent.com/6229665/201674756-0db63ed3-6100-42f1-9e4c-daa2a55b855b.png)

Målinger kan lagres og vises direkte eller fungere som grunnlag for andre arbeidsprosesser, for eksempel journalføring:

![Sammenheng med andre informasjonstjenester](https://user-images.githubusercontent.com/6229665/201674806-5f79126a-2505-4629-83af-69888656f6f9.png)

* Målinger kan legges til i journaldokumenter og journalføres (strukturert eller ustrukturert)
* Hvilke målinger som skal gjennomføres kan styres gjennom egenbehandlingsplanen for pasienten
* Målinger kan inneholde varsel om at målingen ligger utenfor referanseverdien

## Detaljer om egenbehandlingsplan og behandlingsplan

Helsepersonell har uttrykt behov for samarbeid om utarbeidelse og oppfølging av behandlingsplaner og egenbehandlingsplaner. Et slikt samarbeid må fungere med pasient og mellom virksomheter og omsorgsnivå og forutsetter en felles kilde til planen. I tjenesteforløp som inkluderer digital hjemmeoppfølging er det stort behov for koordinering. Dette handler om at pasientene ofte er i kontakt med ulike deler av helsetjenesten og trenger tett oppfølging knyttet til egen sykdom, diagnoser, funksjon og oppfølging av symptomer.
<!-- Det er etterspurt beskrivelse over sammenhenger mellom behandling/egenbehandlingsplan og målarkitekturen -->

## Detaljer om Pasientens legemiddelliste
Helsepersonell som følger opp pasienter i tjenesteforløp der DHO inkluderes etterspør tilgang til en felles legemiddelliste. Tilgang til en felles liste for helsepersonell som følger opp og veileder pasienten kan bidra til å sikre god kvalitet ved behandling med legemidler. Program pasientens legemiddelliste vil etablere en felles digital oversikt over pasientens legemidler, pasientens legemiddelliste (PLL) og PLL vil bli realisert gradvis. 
<!-- Skrive noe om dialogtjenester hvsi tanken er å si noe om de mest prioriterte i informasjonstjenestene -->
<!-- thomiz SVAR: Beskrivelse av utvikling av dialogtjenester må komme på et senere tidspunkt, en annen leveranse -->

<!-- Det er etterspurt beskrivelse over sammenhenger mellom pasientens legemiddelliste og målarkitekturen -->
