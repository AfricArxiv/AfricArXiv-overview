# PKP Open Preprint System

*PKP is a multi-university initiative developing (free) open source software and conducting research to improve the quality and reach of scholarly publishing.* 

For more information go to https://pkp.sfu.ca/ | [PKP Docs Hub](https://docs.pkp.sfu.ca/) | PKP Discussion Forum

In September 2018, [PKP and SciELO Announced the Development of an Open Source Preprint Server System](https://pkp.sfu.ca/2018/09/22/pkp-and-scielo-announce-development-of-open-source-preprint-server-system/).
The Open Preprint System *OPS V3.2 beta* will be launched on Feb 28, 2020. Read [The Road to Preprints (Part 1): Introducing Open Preprint Systems](https://pkp.sfu.ca/2020/02/24/the-road-to-preprints-part-1-introducing-open-preprint-systems/)

OPS pretty much contains and supports all we need for a modern and reliable Open Access preprint service, including: 
- commonly used scholarly types and formats for upload and dissemination, i.e. text-based manuscripts, datasets, presentations etc.
- mutliple languages submission / translations of title, abstract, keywords, etc.
- integration options for ORCID, CrossRef, etc.
- …

## Installation 
Installation should be easy and straightforward, all we need is a server for hosting and a contact person for maintenance and and ensurance of regular updates of the OPS package, whenever PKP releases an update.

The [PKP Web Application Library](https://github.com/pkp/pkp-lib) (PKP-WAL on GitHub) contains all code and descriptions fro OMS, OJS and OPS a.o.
We collect any challenges and suggestions for changes with the software [here as Issues](https://github.com/AfricArxiv/preprint-repository/issues) first try and solve within the AfricArXiv community before approaching PKP. 

---
OPS, empty and unpacked onto a server, is a little under 200MB. The database is relatively small (even with thousands of submissions it should be well under a gigabyte). You'd need to estimate the file storage area for yourself -- this will depend on what format of submissions authors are uploading (e.g. PDF vs. DOCX vs. LaTeX), how big any associated datasets or images are, etc. OPS will maintain a complete copy of these for each version of the submission, so if an author revises a submission after it's been published, creating a new version will double the space it requires.

All in all, the file storage area is the element that will grow most considerably; the rest can be subsumed into a bit of slush factor.

Moving the software from one server to another involves moving 3 things:

The installation directory (the source code, configuration file, etc)
The database (referred to in the configuration file)
The file storage area (referred to in the configuration file)
All of these can be moved as a normal server administration type of task, as long as the configuration file continues to tie all 3 together.

---

## Translations
#### Submissions
PKP OPS supports several languages. Default is English with oppotunities to add translations of titles, keywords and other metadata in sevrral other languages.

#### Interface
The PKP OPS interface will be released with an English, Portuguese and Spanish interface.
Translations to other langauges are aprtially underway and we will mobilize our community to add African translations.

#### Community effort
The PKP translation toolset [Weblate](https://weblate.org/en/) is announced and described at https://pkp.sfu.ca/2020/01/22/introducing-weblate-a-new-path-for-ojs-omp-translations/
Anyone is welcome to work on translations, including starting new ones that will be collected and included with the next releases of the software.
We call on the AfricArXiv community for volunteer translations into African languages; e-mail us to contribute@africarxiv.org PKP Translation User Guide: [OJS/OMP 3.2 Translations with Weblate](https://docs.google.com/document/d/16WvPzofTMPlsTwivo_czEvKWrIQEpdcWyqpgXSbokBQ/edit) (GoogleDoc)


## OJS Usage in Africa: 
Usage statistics are difficult to obtain - no requirement of any kind of registration. 
[This map](https://pkp.sfu.ca/ojs/ojs-usage/ojs-map/) attempts to capture journal counts per country over time. Many more might not be captured but instead to be found anecdotally by looking around Africa. 
The South African numbers are extremely high because that's where [AJOL](ajol.info/) is hosted. 


# Contribute
You can help us get PKP OPS for AfricArXiv off the ground in several ways:
- Help us cover expenses for working hours on https://opencollective.com/africarxiv/contribute/pkp-ops-installation-and-maintenance-14337
- help us translate the submission platform interface into French / Arabic / and most importantly traditional African languages
- assist us in writing user guidelines and finetiune the submission process

Email us at [contribute@africarxiv.org](mailto:contribute@africarxiv.org) to get involved.
