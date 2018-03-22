# OmegaT integration

OmegaT is a translator's workbench, with support for a lot of tools to improve translation speed and quality. But most supported tools are not according to our technologies or needs. We thus want out tools to be integrated smoothly and in such a way that we can deliver a package with everything installed. We want the following integrated:

* spellers (hfst-ospell + zhfst files, or any other lib that can read zhfst files)
* grammar checkers (as an alternative or complement to spellers)
* dictionaries
* terminology lists
* (disambiguated) lemmatisation of words in text
* lemmatised indexes of dictionaries and word lists/terminologies
* corpus search (online, but with results presented in a pane in OmegaT)
* MT is already supported via Apertium (more below)
* most, if not all, should be installable and automatically updated via a Páhkat repo

## Requirements

* solid Java experience
* solid macOS programming experience
* solid Windows programming experience

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work

## Acceptance requirements

Before delivery of final version:

* user documentation
* a working setup with a Páhkat repository, and working installation packages for all components
