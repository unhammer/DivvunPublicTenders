# Grammar Checker integration with MS Office and Google apps

* [Word integration background](Word-integrering.md) (in Norwegian for now)
* [Grammar checker UI and behavior](Spesifikasjon.md) (in Norwegian for now)

## Front-end

The front-end code should be based on the
[GrammarSoft frontend code](https://github.com/GrammarSoft/proofing-gasmso), but reworked so that it can also run offline. More specifically, it needs to store all libraries and components locally, and use them locally, but when there is a network connection, the front-end should check with the back-end server for new versions, and if found, download and install the newer version.

### Targeted platforms/Office versions

* MS Office for Mac
* MS Office for Windows
* MS Office on iPad
* MS Office Online
* Google Apps

## Requirements

* solid C++ programming experience
* solid JavaScript and NodeJS or similar experience
* solid macOS programming experience
* solid Windows programming experience

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work — XXX
* experience with language technology projects
* realistic and sound project plan — XXX

## Acceptance requirements

Before delivery of final version:

* user documentation
* passing all defined tests, on both Windows and macOS
* all code in Github
* code must be language independent
* MS Office integration must work with all language codes, including such codes that are not known to MS Office
* all functionality of libdivvun compiled as a grammar checker must be available via a user friendly and functional User Interface
* the code must follow established styles and linters for the programming language in question
* the code must pass code review by the Divvun group
* the grammar checker must function according to specifications
