# Dictionary apps for mobile phones and pads

## Targeted features

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
* should use majority language speech recognition (Siri, Google Assistant)
  to look up words and expressions to translate
* should use speech synthesis from Acapela (or later: us) to speak out loud
  the translated input words (only SME for now, other languages when voices are available)
* should use open-source OCR libraries and built-in camera to recognice
  printed text and provide translations
* look-up words in text (using morphological analysis (+ disambiguation?) of input string)
* look-up single words / lemmas in the dictionary (standard search)
* dictionary content updated via a Páhkat repository
* the details of the user interface should be worked out in cooperation
  between Divvun&Giellatekno and the company doing the work
* fuzzy match, possibly based on our speller technology, frequency ranked
* Korp lookup if corpus is available, and you have Internnet connection
* paradigm generation (off-line, fst-based)

See also [Mothertoungues.org](http://mothertongues.org/), and the dictionary app released by Språkcentrum in Östersund.

Innhaldsoppdateringar:

* via pahkat
* default: stabil, kvar fjerde veke/ein gong i veka

## Spesifications

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
