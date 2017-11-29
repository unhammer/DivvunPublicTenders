Dette dokumentet er ei skisse til utlysingsprosess og utlysingstekst for
grammatikkontrollintegreringa i Word.

Innleiing
=========

Prosjektet skal levera ein ferdig, fungerande, nordsamisk grammatikkontroll mest mogleg lik MS sin eigen grammatikkontroll. Prosjektet skal byggja på eksisterande grammatikkontrollmodular i form av `divvun-gramcheck` og grammatikkontrollfiler frå `giella-sme`, og integrera desse i MS Office for Windows og macOS. Integreringa skal vera språkuavhengig, og gjera det mogleg å laga grammatikkontrollar for alle språk. All kode for integreringa må vera open kjeldekode, og opphavsretten og eigedomsretten skal ved prosjektavslutning overførast til UiT ved Divvun-gruppa. Overføringa skal vera gjord før siste delbetaling.


Hovudkrav
=========

Korleis skal grammatikkontrollen oppføra seg?

* skal fungera med alle samiske språk
  * sekundært: skal fungera med alle språk vi har (dvs inkl slike som ikkje MS har på lista si)
* skal fungera på Windows og macOS
* dersom han blir bygd med office.js eller tilsvarande teknologi, så må han kunna fungera utan nett
* avsnitt inn, liste med feil attende, kvar feil som start- og sluttpunkt i avsnittet
* støtta forslag; forslaga skal innehalda:
  * kort tittel
  * eitt eller fleire forslag
  * det skal vera mogleg å få ei kort skildring av feilen
  * det skal vera mogleg å få ei lang skildring av feiltypen
* det skal vera mogleg å slå av og på feil som grammatikkontrollen ser etter
  * jf den svenske grammatikkontrollen i Word
* det bør vera (blå? grøn?) understreking under feil
* ein må kunna høgreklikka på feil, og få retteforslag i menyen
* alternativt kan ein visa ein grammatikkontrolldialog
* stavekontrollen vår skal vera ein del av grammatikkontrollpakka
  * det skal vera mogleg å berre ha stavekontroll (mest for å løysa problemet
    med stavekontroll i Word for Mac)
* koden skal vera open
* den ferdige koden skal vera © UiT
* skal byggja på biblioteket laga av [Trigram](https://trigram.no/) i fase 1 av prosjektet

Alt i alt: han skal mest mogleg likna på den vanlege grammatikkontrollen.


Utlysing
========

I heile EU/EØS-området (minst).

Utveljingskriterium
-------------------

1. pris
*  integreringskvalitet (kor mykje liknar det på den *vanlege*
   grammatikkontrollen?)
*  tidlegare røynsle
*  innahusrøynsle i relevante programmeringsspråk
*  tidlegare røynsle med språkteknologiske produkt
*  realistisk prosjektplan
*  økonomisk soliditet?

Akseptanskrav
=============

* koden finst på Github.com/Divvun
* koden byggjer for begge plattformar
* koden passerer alle definerte testar
* koden passerer code review - vi vil ha kode som vi kan halda ved like sjølv
* grammatikkontrollen fungerer etter spesifikasjonane
* enkle grammatikkontrollar for andre språk fungerer, dvs koden er språkuavhengig, inklusive alle språk vi har tastatur eller analysatorar for (dvs slike som ikkje har kode i MS Office)
* all funksjonalitet i libdivvun-gramcheck er tilgjengeleg via funksjonelle grensesnitt
