Skisse til prosjekt for å utvikla mobilklientar for ordbøkene våre.

Eigenskapar
===========

Mobilklientane skal ha desse eigenskapane:

* bruka analysatorane våre (hfst) for lemmatisering + analyse
* vera raske å slå opp i
* enkel og klår typografi
* lettbrukte
* iOS og Android
* ein app for kvart språk, med alle ordbøker til og frå det språket
  * døme:

    Sma-ordboka skal innehalda sma-nob, nob-sma, sma-sme, sme-sma, osb
* ein må kunna slå på og av dei språkpara ein er interessert i
  * døme:

    Om ein ikkje er interessert i sme, må ein kunna slå av sme-sma og sma-sme
* koden skal vera open
* den ferdige koden skal vera © UiT

Utlysing
========

I heile EU/EØS-området.

Utveljingskriterium
-------------------

* pris
* tidlegare røynsle
* innahusrøynsle i relevante programmeringsspråk

Utlysingsdato
-------------

Tentativt hadde det vore bra å ha utlysinga klar til sommaren, med tilbodsfrist
kring midten av august, prosjektstart 1. september. Det hadde sjølvsagt vore bra
å starta før, men eg trur det er urealistisk.

Prosjekttimeplan
================

Eg har definert milepålane i høve til starten, slik at det er lett å justera i
tilfelle vi startar tidlegare eller seinare.

Eg reknar med at dette er ein greid og relativt enkel programmeringsjobb for
gode programmerarar.

1. start:  1. september
2. alfa:   start + 3 mnd
3. beta:   start + 5 mnd
4. ferdig: start + 7 mnd

Akseptansekrav
==============

* koden finst på Github.com/divvun
* koden byggjer for begge plattformar
  * vi skal ha klart å lasta opp ein beta av ei ordbok, og sett at alt fungerer
* koden passerer alle definerte testar

Tekniske spesifikasjonar
========================

Dette omfattar i alle fall:

* ordboksformat
* integrering med analysator (for analyse + lemmatisering)
  * dvs med hfst-lookup eller tilsvarande
* hantering av ikkje-tekstlege data (vil vi ha støtte for det i fyrste versjon?)
* brukargrensesnitt
  * søkjegrensesnitt
  * ordboksartikkel
  * søkjehistorie
  * analyse / lemma
  * vising av (dynamisk) samansette ord
  * vising av (dynamisk) deriverte ord
  * generering av nøkkelformer
  * generering av fullt paradigme
  * visa korpustreff (bør ha ein opsjon for pregenerering, slik at visinga kjem
    raskt; sjå lenger ned)
  * kryssreferansar
  * vising av ulike artikkeldelar (definisjon, omsetjing, døme, etymologi, m.m.)
* integrering med OS-tenester
  * er det mogleg å registrera ordboka slik at ein kan slå opp frå andre appar?
  * delefunksjon (_sjå dette ordet her!_)
* integrering mot andre tenester:
  * talesyntese (for sme, mot vår eigen servar)
  * Korp (kva kan vi gjera for å få Korp-søka raskare?)

Framtidig funksjonalitet
------------------------

* OCR-lesing (med støtte frå hfst-modell) slik at ein kan slå opp ord ved å
  peika på tekst med kameraet
  * er det mogleg å byggja inn Teseract?
  * Finst det andre OCR-lesarar som open kjeldekode?
  * Teseract må trenast på kvar enkelt font, ikkje optimalt
  * sjå <https://en.wikipedia.org/wiki/OCRopus> for eit alternativ

Andre merknader
===============

Vi vil at bygginga skal gjerast automatisk, inklusive signering og anna teknisk
byråkrati. Tanken er at vi skal kunna levera automatiske oppdateringar til faste
intervall (t.d. ein gong i månaden) med dei siste oppdateringane frå termwikien
og andre ordbokskjelder.

Eg meiner vi bør få alle ordbøkene over på ein open redigeringsplattform der
alle kan registrera seg (manuelt - vi vil ikkje ha søppel) og vera med å
redigera. I lag med det førre avsnittet betyr det at folk kan sjå sine eigne ord
etter neste (automatiske) oppdatering. Samtidig bør ordbokskjeldene vera knytte
til fst-ane våre på ein eller annan måte, slik at vi får melding om ord som bør
leggjast til i fst-leksikonet, og omvendt: ord vi har i fst-en som ikkje finst i
ordboka skal finnast som eit tentativt oppslag (men bli ekskludert frå bygginga)
slik at folk ev. kan leggja til omsetjingar, døme, m.m.
