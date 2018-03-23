# Improved CLDR suupport in the keyboard infra

## Locale support
* support for specifying locale data in a simple (yaml) format
* export locale data in CLDR format
* yaml support for Windows specific locale data
* support for building Windows locale installers
* Windows locale installer must be integrated with Windows keyboard installer so that both are installed together

## Improved keyboard support
* export keyboard defs in CLDR xml
* macOS XML import
* improved X11 support
    * read and include existing keyboard defs
    * X11 keyboard def should use include statement + overrides
* support for m17n/ibus
* improved templating based on CLDR data online
* possibly a web-based, graphical editor for the yaml flies
    * needs to display both the yaml content and the layout editor, and data should be two-way synced so that one can edit both

## Requirements

* solid Python experience
* solid macOS programming experience
* solid Windows programming experience
* documented knowledge about locales and keyboards in Windows, macOS and other relevant platforms, in addition to CLDR

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work

## Acceptance requirements

Before delivery of final version:

* user documentation
* passing all defined tests
* all code in Github
