| Status | Version | Maturity | Normative level |
|:-------------|:------------------|:------|:-------|
| <span style="background-color:gold">Work in progress</span> | v0.1 | draft  | ikke normert |

# Slå opp

Samhandlingsformen innebærer at en datatilbyder deler informasjon med en datakonsument på forespørsel. Datatilbyder tilgjengeliggjør informasjonsressurs(er) for deling og datakonsumenten slår opp mot delte dataressurser. Hver aktør har ansvar for produksjon og vedlikehold av egne data, men deler for innsyn fra andre. Denne samhandlingsformen fungerer godt når det ikke er kjent på forhånd hvem som skal ha informasjonen, eller omfanget av dataene er for stort til at det er praktisk å overføre dem samlet. Når en legespesialist ved et sykehus leter etter informasjon i pasientjournalen ved et annet sykehus (for eksempel å slå opp en operasjonsbeskrivelse via dokumentdeling), er dette et eksempel på denne samhandlingsformen. Denne samhandlingsformen kan også brukes på mer strukturerte data (for eksempel kliniske målinger som blodtrykk og puls), såfremt hver aktør har ansvar for produksjon og vedlikehold av sine egne data, og tilbyr innsyn i dem til andre aktører.

[Organisatorisk samhandlingsform: Slå opp (og avgi data)](img/organisatorisk-sla-opp.png)

## Referansearkitektur og målarkitektur for datadeling

I helsesektoren har vi en referansearkitektur og en målarkitektur for datadeling som detaljerer hvordan datadeling i sektoren kan ivaretar deling av helseinformasjon på forespørsel på en sikker måte. Referansearkitekturen beskriver relevante brukertilfeller hvor datadeling kan anvendes og etablerer generelle modeller for tilgangsstyring, API-management og personvern. Målarkitekturen for datadeling beskriver to av brukstilfellene i mer detalj, sektorens samhandling med grunnmur og nasjonale e-helseløsninger og innbyggers samhandling med helse- og omsorgstjenesten.