# Dictionary apps for mobile phones and pads

## Targeted features

* must support iOS and Android
* should use majority language speech recognition (Siri, Google Assistant) to look up words and expressions to translate
* should use speech synthesis from Acapela (or later: us) to read out loud the translated input words (only SME for now, other languages when voices are available)
* should use open-source OCR libraries and built-in camera to recognice printed text and provide translations
  * Teseract? Other open-source OCR libraries?
  * Teseract needs to be trained on every font, not optimal
  * see [OCRopus ](https://en.wikipedia.org/wiki/OCRopus) for an alternative
  * instead of an OCR library one can use OS services, if available
* look-up words in text (using morphological analysis (+ disambiguation?) of input string)
    * preferably using OS services if available
* look-up single words / lemmas in the dictionary (standard search)
* dictionary content updated via a Páhkat repository
    * default: stable channel, check every week
* the details of the user interface should be worked out in cooperation between Divvun&Giellatekno and the winning tenderer
* fuzzy match, possibly based on our speller technology, frequency ranked
* Korp lookup if corpus for the language is available, and Internet connection is available
* paradigm/word form generation (off-line, fst-based)
    * key forms
    * full paradigm
    * which one to generate should be a user preference, or possibly a two-step process: always generate the key forms, then if the user taps on an expansion triangle or somesuch the full paradigm should be displayed
* speedy, fast lookup of dictionary entries
* clear and easy-to-read typography
* easy to use
* should use the same XML format as the other dictionary platforms as input at buid time (but internal representation can of course be different)
* support for audio, video, images as part of dictionary entries
* search history
* when looking up compound words in text that are not found in the dictionary, the app should present the articles for the compound constituents. The same goes for derivations
* cross reference lookup
* hiding / showing different parts of dictionary articles (e.g. etymology, examples, homonyms, synonyms, etc.)

Whether to build one app for each language (containing dictionaries to and from that language), or build one language with all dictionaries installed is presently left unspecified. In any case it must be possible to turn off dictionaries and language pairs the user is not interested in.

See also [Mothertoungues.org](http://mothertongues.org/), and the dictionary app released by Språkcentrum in Östersund (link forthcoming).

## Requirements

* solid iOS and Android programming experience
* solid mobile and pad UI experience

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with dictionary app development

## Acceptance requirements

Before delivery of final version:

* technical documentation
* passing all defined tests
* all code in Github

<!--
Andre merknader
===============

Vi vil at bygginga skal gjerast automatisk, inklusive signering og anna teknisk
byråkrati. Tanken er at vi skal kunna levera automatiske oppdateringar til faste
intervall (t.d. ein gong i månaden) med dei siste oppdateringane frå termwikien
og andre ordbokskjelder.

Eg meiner vi bør få alle ordbøkene over på ein open redigeringsplattform der
alle kan registrera seg (manuelt - vi vil ikkje ha søppel) og vera med å
redigera. I lag med det førre avsnittet betyr det at folk kan sjå sine eigne ord
etter neste (automatiske) oppdatering. Samtidig bør ordbokskjeldene vera knytte
til fst-ane våre på ein eller annan måte, slik at vi får melding om ord som bør
leggjast til i fst-leksikonet, og omvendt: ord vi har i fst-en som ikkje finst i
ordboka skal finnast som eit tentativt oppslag (men bli ekskludert frå bygginga)
slik at folk ev. kan leggja til omsetjingar, døme, m.m.
-->
