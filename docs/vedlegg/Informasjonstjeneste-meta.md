---
title: Informasjonstjeneste metamodell
---

| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
| <span style="background-color:BlueViolet">Prerelease</span> | v0.9.1 | review | ikke normert |

Et sentralt begrep i forbindelse med helhetlig samhandling og målarkitekturen for datadeling innen DHO er informasjonstjeneste. I sin grunnleggende form er en informasjonstjeneste definert:

!!! note "Informasjonstjeneste"
    
    Informasjonstjenester, er en samlebetegnelse for alle typer tjenester som tilbyr eller manipulerer informasjonsressurser i form av en definert tjeneste.

Dette kan modelleres på denne måten:  

[![Modell som viser informasjonstjeneste som brukt i samhandling. Archimate modell.](../img/Informasjonstjeneste-enkel.png){width="500"}](../img/Informasjonstjeneste-enkel.png)
*Enkel fremstilling av informasjonstjeneste i forbindelse med samhandling*

En informasjonstjeneste kan skrive og lese informasjon i form av informasjonsressurser. Informasjonstjeneste kan understøtte Forretningsprosesser direkte eller indirekte som en del av en Samhandlingsprosess. Informasjonstjenester realiseres vanligvis som mer spesifikke applikasjonstjenester (tjenester for datadeling, meldingsutveksling eller dokumentdeling).

## Helhetlig samhandling

I forbindelse med arbeidet for å tilrettelegge for helhetlig samhandling er det kartlagt en rekke informasjonstjenester det er behov for. På øverste nivå defineres informasjonstjeneste på denne måten med fokus på samhandling.

!!! note "Informasjonstjeneste i helhetlig samhandling"
    
    En informasjonstjeneste er en gruppering av informasjon/informasjonsbehov som kan deles mellom innbygger, helsepersonell og andre aktører via samhandlingsløsningene.

En definisjon av alle de ulike informasjonstjenestene som ble beskrevet i forbindelse med helhetlig samhandling ligger i kapittel 4 i [Bilag G2: Helhetlig samhandling (PDF)](https://www.ehelse.no/publikasjoner/sentralt-styringsdokument-akson-helhetlig-samhandling-og-felles-kommunal-journallosning/Bilag%20G2%20Helhetlig%20samhandling.pdf). I sin beskrivelse av de ulike informasjonstjenestene blir flere egenskaper beskrevet:  

* Aktører som har behovet.
* Informasjonsbehov som understøttes av informasjonstjenesten.
* Sammenheng med andre informasjonstjenester.
* Deltjenester for å ivareta sammensatte informasjonsbehov.
* Brukerhistorier som understøttes av informasjonstjenesten.
* Relevante standarder for realisering.

Dette fører til en mer kompleks metamodell for informasjonstjenester i forbindelse med helhetlig samhandling.

[![Metamodell for informasjonstjenester i helhetlig samhandling](../img/informasjonstjeneste-metamodell.png)](../img/informasjonstjeneste-metamodell.png){width="600"}

I arbeidet med målarkitektur for datadeling innen DHO er det den komplekse modellen vi forholder oss til. Det vil si at vi legger beskrivelsene av de ulike informasjonstjenesten til grunn når vi analyserer informasjonsbehovet i tilknytning til DHO.
