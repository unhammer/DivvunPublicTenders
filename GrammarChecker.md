# Grammar Checker integration with MS Office and Google apps

This subproject should take our grammar checker library and turn it into a functional grammar checker tool for MS Office and Google apps users, resembling the standard MS Office grammar checker as much as possible.

## Front-end

The front-end code should be based on the
[GrammarSoft frontend code](https://github.com/GrammarSoft/proofing-gasmso), but reworked so that it can also run offline. More specifically, it needs to:

* store all libraries and components locally, and use them locally
* when there is a network connection, the front-end should check with the back-end server for new versions, and if found, download and install the newer version
* it should also be possible to run the grammar checker completely server-based, in cases where it is not possible to store files locally, or running the grammar checker locally turns out to be too heavy on the platform according to some test
* the front-end must run server-based while downloading support files, so that end users don't have to wait for the download to finish before starting the grammar checker

Functional requirements:

* send and receive a paragraph of text to the back-end, and receive a list of errors such that they can be marked in the source text or highlighted in the grammar checker user interface
* present correction suggestions containing the following:
    * short error title
    * one or more correction suggestions
    * a short description of the error(s)
    * based on user action, also a long description of the error
* it must be possible to turn on or off checking of specific grammar errors (the list of available errors is given by the backend); cf. also the [Swedish grammar checker in MS Word](Spesifikasjon.md)

### Targeted platforms/Office versions

* MS Office for Mac
* MS Office for Windows
* MS Office on iPad
* MS Office Online
* Google Apps

## Back-end

The backend should be based on existing backends, and the communication between back-end and front-end should be similar to already working solutions. — XXX which one?

The back-end must be a wrapper around [libdivvun](https://github.com/divvun/libdivvun) compiled as a grammar checker library. The back-end must:

* support uploading of libraries and support files so that the front-end can run off-line
* support version checking of libraries and support files, to facilitate uploading of new versions compared to what is already on the client

The interface should also follow whatever the REST/GraphQL subproject settles on.

## Further details

* [Background and functional definition](Word-integrering.md) (in Norwegian for now)
* [UI and behavior](Spesifikasjon.md) (in Norwegian for now)


## Requirements

* solid C++ programming experience
* solid JavaScript and NodeJS or similar experience
* solid macOS programming experience
* solid Windows programming experience

**solid** = reference to at least five independent projects involving the programming language or platform in question.

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
