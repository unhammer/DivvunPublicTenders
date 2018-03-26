This subproject concerns the possible replacement, upgrade and/or further development of [satni.org](http://satni.org/).

## Background

[Satni.org](http://satni.org/) is a portal for publishing and presenting electronic dictionaries and terminology for the Sámi languages. It differs from other web dictionaries provided by the Divvun and Giellatekno groups in the following ways:

* it includes the content of the [Sámi TermWiki](https://satni.uit.no/termwiki) (i.e. terminology)
* it presents all dictionaries for all language pairs in one unified interface
* all dictionary entries for a given word or search term is displayed at the same time, with a header separating and identifying each dictionary or term collection
* satni.org is developed in cooperation with the [Norwegian Sámi Parliament](https://samediggi.no/) and [Giellagáldu](http://www.giella.org/) (other dictionary interfaces are developed independently at UiT)

All dictionaries and term collections are stored in a common XML format.

The present solution is using the [eXist indexed XML database](http://exist-db.org/) as a backend, and a Javascript web app as a front end. The present code for the whole system is available in [our svn repository](https://gtsvn.uit.no/langtech/trunk/apps/risten2/).

## Targets

The following areas should be addressed by the tender:

* speed
* responsiveness of web UI
* adaption to use on mobile devices & different screen sizes
* integration with other services via the REST/ GraphQL API (see that subproject in the tender documents), including at least:
    * paradigm generation (**new**)
    * speech synthesis (**new**)
    * corpus searches (**existing**)

Whether to replace or keep the present backend is up to the tenderer. Preferably both altnernatives should be presented, with a price tag for each.

As the Norwegian Sámi Parliament is a stakeholder in the project, they should also be involved in the development project via regular meetings and discussions related to functionality and user interface. The Divvun group is responsible for organising such meetings, and to ensure appropriate communication between the tender winner and the Sámi Parliament.

## Requirements

* solid XQuery or alternate backend query language experience
* solid Javascript programming experience
* solid webapp building experience
* solid experience with user interface design for various screen sizes

**solid** = reference to at least five independent projects involving the language or platform in question.

## Subproject selection criteria

* experience with similar work

## Acceptance requirements

Before delivery of final version:

* technical documentation
* web app accepted by the Norwegian Sámi Parliament
* passing all defined tests
* all code in Github or svn
