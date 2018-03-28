# Grammar checker background and functional definition

This subproject should deliver a finished, fully functional North Sámi grammar checker resembling the standard MS Office grammar checker as much as possible.

Hovudkrav
=========

* må kunna senda avsnitt inn til divvun-gramcheck-biblioteket og tolka ei returnert liste med feil, der kvar feil refererer til start- og sluttpunkt i avsnittet
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
