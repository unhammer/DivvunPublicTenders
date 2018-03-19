# Graphical text analysis application for linguists

* paste text, get analysed text in a different window/pane:
    * trestruktur
    * Ulike alternativ for formattering av analysen
    * kopier analysen i passande format, slik at ein enkelt kan lima inn i andre program (som døme når ein skriv artiklar m.m.)
testing og vurdering av programmet
* automatisk oppdaterte språkpakker via Páhkat
* a graphical wrapper around libdivvun + zcheck files:
    * text used as input to libdivvun in one pane
    * output appears in the other pane
* versjon både for mac, win og linux
* jf [Apertium Simpleton](http://wiki.apertium.org/wiki/Apertium_Simpleton_UI)

GUI mockup:

![Mockup interface](bilete/AnalAppMockup.png)

# Notes

* the Analysis popup menu is just a listing of the available pipelines for the selected language, as returned by libdivvun
* Output format is a list of whatever final reformatting we choose to provide as part of the app — it should at be a reasonable selection of formats, like:
    * Giella (a «raw» format)
    * UD
    * common formats used in scientific literature
* the default format should be setable in the app settings
* the mockup above is in no way binding, it is just to visualise the basic functionality of the app

# Target user group

Linguists and researchers wanting to use our analysis tools without having to compile and set up a large number of different things. This app (obtained via the Páhkat clients) should be a one-stop-get-it-all for researchers interested in the languages in the Giella infra.

# Possible future extension

* tool or interface to provide user feedback - missing words, wrong analyses, etc
* one pane for each analysis step?
    * each pane could be editable, so that corrections can be made, and the corrected data would then be used as input for the subsequent processing steps/panes?
