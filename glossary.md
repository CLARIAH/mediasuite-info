---
layout: page
title: Glossary
---

## Alignment

By Roeland Ordelman

Alignment (officially ‘forced alignment’) is the process of  synchronizing a text transcription of speech to the audio recording that  contains the speech, by automatically adding time labels to every word  in the transcript using a specific form of speech recognition  technology. This technology is sometimes called ‘informed speech  recognition’: the words to be recognized are already known — the task is  to find the exact positions in the audio where the words occur. In  practice, the speech transcripts are usually not an exact representation  of the speech. For example, repetitions and filler words such as ‘uh’  and ‘ah’ are often omitted, and ungrammatical sentences reformulated.  The further the text transcripts depart from the verbatim speech, the  more difficult the alignment process for the speech recognition  technology will be.

Alignment is a very valuable tool to enable word level access to  spoken word recordings (jump to positions where a particular word is  mentioned) in cases where text transcripts are available such as in Oral  History research where scholars are used to making verbatim transcripts  of interviews in word processors that do not capture time information.   Examples of text transcripts in other domains that are deployed for  alignment are subtitles for the hearing impaired, auto-cues, production  scripts, and court reports.

An alignment tool typically takes as input (i) a plain text file with  the speech transcript, and (ii) the audio recording that contains the  speech, and provides as output a file where time labels are added to  each of the words in the transcript, for example in a list format with  on each line the start time and a word:

00:01:23:34 today

00:01:25:01  we

00:01:25:28 started

This output can be used in a transcription viewer to  jump  immediately to the corresponding position in the audio file by clicking  on a word while viewing a single interview. It can also be used to jump  to positions in multiple audio files by indexing the aligned text (of  multiple interviews) in a search engine.

See more at this blog post about the [CLARIN-Plus workshop on oral history](https://clariah.github.io/mediasuite-blog/blog/2017/05/12/CLARIN-PLUS-workshop-on-Oral-History).

## API

## ASR

## AVResearcher

"In [AVResearcherXL](http://labs.beeldengeluid.nl/application/dbd09298-edb3-11e4-8099-005056a71e3a) kunnen onderzoekers vergelijkend onderzoek doen tussen radio- en televisiemateriaal en geschreven nieuwsmedia. De tool bestaat uit twee identieke zoekboxen die eigen word clouds, histogrammen en resultatenlijsten genereren, en uit een tijdslijn waar resultaten gecombineerd kunnen worden weergegeven. Door de aanwezigheid van ondertitels spraaktranscripten gedigitaliseerde digitale kranten wordt AVResearcherXL wordt onder andere gebruikt voor onderzoek naar representatie, beeldvorming en discours." (Source: previous CLARIAH website, 2016)

This tool is no longer maintained by CLARIAH, but the same functionality, with extended data is to be performed with the [[Compare]] tool.

## CKAN

## Classification

## Collection

## CoMeRDa

"In de zoekmachine CoMERDa (Contextualized Media Research Data) kunnen radio- en televisiecollecties samen met bronnen over de productie, programmering en publieke omroepgeschiedenis getrapt en tegelijkertijd worden doorzocht. Vanwege auteursrechtelijk beperkingen is CoMerDa alleen beschikbaar binnen de muren van het Nederlands Instituut voor Beeld en Geluid." (Source: previous CLARIAH website, 2016).

**Note**: This tool is not maintained as such by CLARIAH. Instead, extended collections and functionalities can be used via the Media Suite.

## Data dump

## DIVE+

"DIVE is een op historische gebeurtenissen gebaseerde zoekbrowser die openbare data uit musea en bibliotheken toegankelijk, exploreerbaar en navigeerbaar maakt voor onderzoekers en het grote publiek. Dit gebeurt door middel van het automatisch koppelen van metadata over (onder andere) plaatsen en personen. In DIVE+ wordt gewerkt aan een uitbreiding hiervan. DIVE+ geeft onder andere inzicht in de manier waarop automatische kopelingen tussen digitale (media-)erfgoedbronnen mede bepalend zijn voor onze (re)constructies van de geschiedenis. Voor beide versies zijn geen inloggegevens nodig. Meer informatie vind je op het DIVE blog." (Source: previous CLARIAH website, 2016).

**Note**: [DIVE](http://labs.beeldengeluid.nl/application/dbd0184a-edb3-11e4-8099-005056a71e3a) is an experimental tool created by researchers at the Vrije Universiteit (and [Frontwise](https://www.frontwise.com/)) to generate and use linked data for cultural heritage in a user-oriented interface. The DIVE project has generated significant research and expertise in this domain (see the [DIVE project blog](http://diveproject.beeldengeluid.nl/)). In CLARIAH overall, and in the WP5's Media Suite, there is ongoing work in integrating linked data with ES indexes, in a standardized and sustainable way, to make it aligned with the ongoing efforts of CLARIAH's ANANSI (see [[FAQ: How does the Media Suite make the data available?]]). The DIVE tool (its methods for converting and enriching linked data, and the graphic user interface) is then being integrated progressively into the CLARIAH infrastructure.

## Entity

## ES (Elastic Search)

## Exploration path

## GTAA

## Gitter

## JSON

JSON (JavaScript Object Notation) format, which is a ubiquitous internet data interchange format.

## Jupyter Notebooks

## Metadata (card)

## OAI-PMH

## QDA

## Query

## Recipe

## Resource viewer

## Transcription

By Roeland Ordelman

Transcription is the systematic representation in written form of  language: speech, sign language, or text in another writing form. In the  academic discipline of Oral History research, transcription is an  essential part of the methodology, as the transcripts are the main  source for analysis of the Oral History interviews. In recent times,  tools such as alignment are emerging that allow Oral History scholars to  simultaneously use text transcripts and the original audio recordings  during analysis. Outside academia, examples of transcriptions are the  proceedings of court hearings or physician’s recorded voice notes. A  verbatim transcript includes all dialogue spoken, word for word,  including fillers, false starts, and repetitions.

Automatic speech recognition (ASR) technology is increasingly used to  support or even replace manual transcription. As speech recognition  will produce errors that need to be corrected manually afterward,  specialized tools are developed that try to make the correction work  less tedious.

See more at this blog post about the [CLARIN-Plus workshop on oral history](https://clariah.github.io/mediasuite-blog/blog/2017/05/12/CLARIN-PLUS-workshop-on-Oral-History).

## Trove

"TROVe stelt wetenschappers in staat stelt om de verspreiding van nieuws, opinie en debat  te analyseren in verschillende media door de tijd heen. Hiermee kunnen de bijdragen van en onderlinge relaties tussen massamedia en nieuwe (sociale) media onderzocht worden. TROVe geeft inzicht in de manieren waarop media, informatie en individuen het digitale tijdperk verbonden zijn, hoe zij het publieke debat bepalen, en hoe zijn erdoor bepaald worden. Helaas is TROVe vanwege rechten- en serverbeperkingen niet meer beschikbaar tot aan zijn intergratie in de Media Suite. [Bekijk hier wel de screencast uit 2013](https://www.youtube.com/watch?v=EWx0xAFRlA0&feature=youtu.be)."

[More information about TROVe here](http://labs.beeldengeluid.nl/application/dbd0b3e0-edb3-11e4-8099-005056a71e3a).

**Note**: This tool is not maintained as such by CLARIAH. Instead, extended collections and functionalities can be used via the Media Suite.

## Unesco thesaurus

## User project

A "User project" is a sort of container for storing personal corpora and annotations created during search and analysis of the data available in the Media Suite.  Some of the Qualitative Data Analysis (QDA) typically used by researchers, refer to user projects as "hermeneutic units" (in Atlas.ti) or "Projects" (in NVIVO). For instance, a researcher can create a user project for a topic or for a research question, which will help her/him to group together entire items or fragments for creating a corpus (the so-called "bookmarks"), manual annotations, queries, browsing history and "tool sessions: from the Exploratory tool (the so-called "navigation paths"), among others.

## Verteld Verleden

"[Verteld Verleden](http://labs.beeldengeluid.nl/application/693621d8-2a1e-11e5-b980-005056a71e3a) brengt (meta)data en spraaktranscripten van tientallen oral history-collecties verspreid over Nederland bij elkaar en maakt deze doorzoekbaar op basis van gedetailleerde zoek- en filteropties. De tool bevordert daarmee de toegankelijkheid en doorzoekbaarheid van deze unieke collecties. Geen inloggegevens vereist."

This tool is not maintained as such by CLARIAH. Instead, extended collections and functionalities can be used via the Media Suite.