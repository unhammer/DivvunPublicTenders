# Graphical text analysis application for linguists

* paste text, get analysed text in a different window/pane:
    * syntactic tree structure/dependency tree
    * there should be different formatting/rendering options for the analysis
      output (see mockup below)
    * it should be possible to copy the displayed analysis in a suitable format
      (specified in the app settings), so that one can easily paste it into
      other applications, e.g. when writing academic papers
* analysers/processing pipelines (one pr language) should be automatically
  updated via the Páhkat repository
    * does this mean that we need/want a Páhkat client for Linux? Or could it be
      embedded in the GUI app if this is the only use case for Páhkat on Linux?
* the app is essentiallly a graphical wrapper around libdivvun + `zcheck` files:
    * text used as input to libdivvun in one pane
    * output appears in the other pane
    * processing is done as specified in the `zcheck` file for the given
      language
* the application should be made for all of macOS, Windows and Linux using
  native code for the UI parts. No generic UI libraries should be used!
  This is done to get application behavior and look&feel that properly follows
  the guidelines and user expectations of each platform

Also have a look at
[Apertium Simpleton](http://wiki.apertium.org/wiki/Apertium_Simpleton_UI) for
inspiration.

GUI mockup:

![Mockup interface](bilete/AnalAppMockup.png)

# Notes

* the **Analysis** popup menu is just a listing of the available pipelines for the selected language, as returned by libdivvun
* **Output format** is a list of whatever final reformatting we choose to provide as part of the app — it should at be a reasonable selection of formats, like:
    * Giella (a «raw» format)
    * UD
    * common formats used in linguistic litterature
    * the *default* format should be setable in the app settings
* the **Language** popup must list all and only the languages returned by libdivvun
* the mockup above is in no way binding, it is just to visualise the basic functionality of the app
* the file suffix `zcheck` is used in this specification for the file containing the linguistic data and the actual pipeline specifications, as that is the suffix used for a similar pipeline file for grammar checking. In the final app the file suffix will most likely be different.
* command line interface, to allow piping text into it, possibly also analysis results out of it
* other possible functionality:
    * display more morphophonological info and other info based on lexc entry
    * Korp searches triggered from analysis window (e.g. to see other uses of the lemma)
    * extract frequency lists? Other linguistic analysis tools?

See also the
[Oslo LAP](https://www.mn.uio.no/ifi/english/research/projects/clarino/) web
app.

# Target user group

Linguists and researchers wanting to use our analysis tools without having to compile and set up a large number of different things. This app (obtained via the Páhkat clients) should be a one-stop-get-it-all for researchers interested in the languages in the Giella infra.

# Possible future extension

* tool or interface to provide user feedback - missing words, wrong analyses, etc
* one pane for each analysis step?
    * each pane could be editable, so that corrections can be made, and the corrected data would then be used as input for the subsequent processing steps/panes?
