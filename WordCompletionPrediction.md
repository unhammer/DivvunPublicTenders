
# Word completion and prediction for the Giella mobile keyboards

* target platforms: iOS and Android
* possibly in cooperation with the Hfst team at Helsinki University and/or a development team in Canada, organised through AltLab at the University of Alberta

## Word completion

* some sort of lemma, morphology and word form frequency weighting
* fst-based, essentially adding a star to the end of the string typed so far, and suggesting the best match in the fst
* possibly combined with a trigram model looking at the two previous words (can only be done on iOS as long as we cache the input — there is no way to access the text buffer beyond the present word)

## Word prediction

Probably something along the following lines:

* trigram model of word forms
* trigram model of lemma / POS / inflections

## Requirements

* solid Rust programming experience
* solid iOS programming experience
* solid Android programming experience

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work — XXX

## Acceptance requirements

Before delivery of final version:

* user documentation
* passing all defined tests
* all code in Github
