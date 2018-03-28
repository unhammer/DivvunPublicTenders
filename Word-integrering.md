# Grammar checker background and functional definition

This subproject should deliver a finished, fully functional North Sámi grammar checker resembling the standard MS Office grammar checker as much as possible within a number of given constraints.

Prosjektet skal levera ein ferdig, fungerande, nordsamisk grammatikkontroll mest mogleg lik MS sin eigen grammatikkontroll. Prosjektet skal byggja på eksisterande grammatikkontrollmodular i form av `libdivvun` og grammatikkontrollfiler frå `giella-sme`, og integrera desse i MS Office for Windows og macOS. Integreringa skal vera språkuavhengig, og gjera det mogleg å laga grammatikkontrollar for alle språk. All kode for integreringa må vera open kjeldekode, og opphavsretten og eigedomsretten skal ved prosjektavslutning overførast til UiT ved Divvun-gruppa. Overføringa skal vera gjord før siste delbetaling.


Hovudkrav
=========

* skal fungera med alle språk, inkl slike som ikkje MS har på lista si
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
