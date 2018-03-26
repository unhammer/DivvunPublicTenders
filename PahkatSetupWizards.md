# Setup Wizards for the Páhkat clients

This subproject should add a new feature to the Páhkat clients for [Windows](https://github.com/divvun/pahkat-client-windows) and [macOS](https://github.com/divvun/pahkat-client-macos). The new feature is a first-time setup wizard that:

* runs first time (or on request)
* asks for languages of interest
* asks for tools of interest
* downloads and installs the selected tools/components (and all dependencies)
* make the clients only show the selected language(s) in the main window (ie hide the languages not relevant to the user)
    * (or show them under some sort of *other* category)
    * language set can be changed later in settings window
    * notify user of new tools for the selected language(s)

## Requirements

* solid macOS programming experience
* solid Windows & Inno Setup programming experience

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work

## Acceptance requirements

Before delivery of final version:

* user documentation
* passing all defined tests
* all code in Github
