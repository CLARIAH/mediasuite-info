---
layout: page
title: Frequently Asked Questions (FAQ)
---
## What is the Media Suite?

The Media Suite is a "virtual research environment" (VRE) within the Dutch infrastructure for digital humanities and social sciences [(CLARIAH)](https://clariah.nl/), which aims to serve the needs of media scholars, oral historians, and other scholars working with audiovisual data collections and related multi-media contextual sources that are maintained at cultural heritage and knowledge institutions.

The CLARIAH Media Suite is a constantly evolving VRE that follows the principles indicated by Candela et al (2013):

"*Virtual Research Environments are innovative, web-based, community-oriented, comprehensive, flexible,and secure working environments conceived to serve the needs of modern science.* "[^1]

[^1]: Candela, L., Castelli, D., & Pagano, P. (2013). Virtual Research Environments: An Overview and a Research Agenda. *Data Science Journal*, *12*(0). <https://doi.org/10.2481/dsj.GRDI-013>.

In our case, the aim is to serve the needs of "digital" humanists and social scientists, mostly in The Netherlands, but in close link with international initiatives, such as [DARIAH](https://www.dariah.eu/) and [CLARIN](https://www.clarin.eu/).

## How can I access the Media Suite?

The CLARIAH Media Suite needs to operate with an authentication service. This means that users have to log in to use most of its services. This is necessary since many of the collections that are offered in this environment are copyrighted or have access restrictions due to privacy. 

CLARIAH outsources this authentication service to [SurfConnext](https://www.surf.nl/en/services-and-products/surfconext/index.html), a service offered by SURF, which is the collaborative ICT organisation for Dutch education and research.

Via this service, students, teachers and researchers with a valid institutional account use  SURFconext to log in to the Media Suite. They can do so securely and easily using the account issued  by their own institution.

**Note**: The aim of CLARIAH is to offer open services to researchers. In Version 3, authentication via SURFConext is required to enter all data and services of the Media Suite. In future versions, we aim to remove some of this authentication requirements to make it possible to use our open source tools with the collections/data that is open. When this is in place, no login will be needed to use the tools with the non-restricted data sets.

These are the steps for this authentication:

1. Go to [the Media Suite](http://mediasuite.clariah.nl/)
2. Click on the "Log in" button at the top right of the page
3. In the SURFConext interface, search for the name of your institution, or scroll through the list
4. Select your institution
5. Use your institutional credentials to log in, wait until the service connects
6. You will arrive at the CLARIAH Media Suite workspace [[read further documentation about the workspace]]

> See at our CLARIAH YouTube channel the [Screencast: How to log in to the Media Suite](https://www.youtube.com/watch?v=2z0xUblnZwo&index=1&list=PLM8OWdLwjOmcOOikb_vCgB3ouY98PKvge)

The following are situations in which you may not be able to use the Media Suite at this moment:

- **When your institution name does not appear in the list of SURFConext institutions**: This happens when you are prompted to the login page of The Media Suite, you search for your institution in the search box, and your institution is not listed there. Most academic and research institutions in the Netherlands are connected with SURFConext. If your institution is not in the list, this means your institution is not connected. This issue has to be solved by the <u>Dutch</u> university or research institution to which the researcher belongs to. Your institution also has to connect to the CLARIN service (that the Media Suite belongs to), in the local SURFconext settings. If your institute is not listed in the Media Suite, you have to ask your local ICT helpdesk to make this connection. Every institution has one or more SURFcontext maintainers/responsibles who should be able to do this for you.
- **When you don't have a Dutch institutional affiliation**: This happens when you find the institution in the SURFconext list, but you don't have valid credentials to log in. In Version 3 is currently not possible to authenticate and use the Media Suite if you don't have valid institutional credentials. We are working towards providing an authentication solution for this case in future versions. A solution to this, may be to ask a host institution listed in the SURFConext institutions to create a temporary institutional account for you.
- **When a non-Dutch institution wants to have access to the Media Suite**: This is currently not possible in Media Suite version 3. A possible solution to this, may be to ask a Dutch host institution listed in the SURFConext institutions to create a temporary institutional account for you.

## What kind of data is available via the Media Suite?

The Media Suite aggregates metadata from audiovisual collections and related multi-media contextual sources that are maintained at cultural heritage and knowledge institutions in The Netherlands. In Version 3, the Media Suite offers simultaneous (but not integrated) access to 9 collections (grouped by provider):

**The Netherlands Institute for Sound and Vision**

- The audio-visual collection (most resources can be played via The Media Suite. In Version 3 this requires an additional step -see [[FAQ: Can I play/view all the resources...]] )
- The television collection (same as above for access to the resources)
- The radio collection (same as above for access to the resources)

**The EYE Filmuseum's Jean Desmet collections**

- The film collection (all items, ca. 800 of the Desmet film collection can be played from EYE servers via the Media Suite)
- The poster collection (most posters of the Desmet poster collection can be viewed from EYE IIIF servers via the Media Suite)
- The paper (business archive of Jean Desmet) collection (all digitized papers of the Desmet business archive can be viewed from EYE IIIF servers via the Media Suite)

**DANS (Data Archiving and Networked Services)**

- A big part of the metadata of oral history collections  from DANS (in Version 3 access to the media resources is only possible to the "open open" access collections)

**A collection from the National Library of The Netherlands (KB)**

- The KB's newspaper "basic" collection (all metadata from the [[KB newspapers basic collection]] can be accessed via the Media Suite, the resources themselves, can be viewed/accessed via a re-direct to the KB system [[Delpher]])

**Open Images (Open Beelden) project collections**

- The EYE Open Beelden collection (all metadata and resources from this open access collection can be accessed and played)
- The Sound and Vision Open Beelden collection (all metadata and resources from this open access collection can be accessed and played)

## How does the Media Suite make the data available?

Technically, the integration of the metadata into the Media Suite is done either:

1. By using the [[APIs]] of the content providers (when available)
2. By harvesting the metadata exposed via [[OAI-PMH]] protocols (when available), or,
3. Via [[data dumps]].

Accessing the media resources (videos, audio, images, text) works in a different way. In most cases, these objects are hosted by the [contributing institutions or projects](http://mediasuitedata.clariah.nl/group), and the Media Suite provides access to "playout" or "viewing" functionality either inside the [[Resource viewer]], or by redirecting the users to the original provider (this is done, for example, in the case of the KB newspaper collection).

Since one of the aims of CLARIAH is to encourage and support institutions to make their data available to researchers, in any of these cases, data provision is done in collaboration between CLARIAH and the [contributing memory institutions or projects](http://mediasuitedata.clariah.nl/group). Developers, scholars, and the curators from the institutions providing these data to be accessed via the CLARIAH Media Suite have been working together to make collections available via the Media Suite.

From the technical perspective, the Media Suite works with documents expressed in [[JSON]] format. These documents are stored in [[ElasticSearch]] (ES) indexes, which can be search and retrieved using Lucene (a free and open source information retrieval software library). The strengths of ES are the support to faceted search and full text retrieval. 

In parallel, there is ongoing work in converting all collections available via the Media Suite to JSON-LD documents (linked open data). This is with the aim to facilitate future integration with ANANSI [[Data]], the CLARIAH linked data central connection of all datasets. In version 3, the Media Suite offers only one experimental collection in JSON-LD (Open Images from The Netherlands Institute for Sound and Vision). This collection can be browsed using the [[Exploratory search tool]]. The “media objects” available in this way, are connected to the ES indexes, thus, users can seamlessly search and navigate this collection in both the ES-based Media Suite tools and the linked-data based exploratory tool.

## Can I play/view all the sources that I find via the Media Suite?

The Media Suite provides access to data from different institutions ([data providers](http://mediasuitedata.clariah.nl/group)), but does not host all the media resources (e.g., videos, images, documents). When you find a resource that is not viewable/playable this may be due to three reasons:

1. The resource may not have been digitised. In these cases, you can consult the metadata, but you cannot view the content. In the [[Search tool]], you will find in these cases an icon with a closed eye, you should consult the metadata in the [[Resource viewer]] to identify if the item is not digitised. A way to solve this is to contact (or visit) the the providing institution.
2. The resource may be digitized, but not have been made available by the content provider to be played or viewed via the Media Suite. This can happen in the case of privacy or copyright restrictions. In Version 3, this case is most frequent in for the DANS oral history collections. In this case, you will find a closed eye icon next to the resource in your result list.
3. The resource may have been made available by the content provider, but with certain additional security. In Version 3, this case applies to the collections provided by The Netherlands Institute for Sound and Vision. To play or view their content, you will have to request a VPN connection (use our [[contact information]], which has to be used even after being logged in to the Media Suite.

See more information under the [[FAQ: What kind of data is available via the Media Suite?]].

## How does the CLARIAH Media Suite work?

- From a user perspective, the CLARIAH Media Suite is a "virtual research environment" (VRE) with a user-friendly interface (plus other more advanced services to work with data directly). 

  It enables users to access important Dutch audio-visual collections and their related sources via search and browsing tools. The embedded functionalities for bookmarking and annotating allow users to save their corpora and perform more detailed annotations and enrichments with these corpora. 

  Ideally, users start by creating a so-called "[[User project]]", to which they can add bookmarks, annotations, queries, navigation paths, and tool sessions. This helps users to do basic analysis work of the sources in the Media Suite's workspace, and keep track of their work progress over time. The basic exporting features allow users to combine and query these corpora, their enrichments and annotations. 

  Because user-friendliness can limit flexibility of more advanced users in working with the actual data, we include in Version 3 a number of experimental [[Jupyter notebooks]] to enable users with some level of python knowledge to perform more advanced processing of the data offered in the Media Suite. In any case, because most of the collections that are offered in this environment are copyright-protected or have privacy restrictions to be exported or shared, users have to log in to work with these data, also with the [[Jupyter notebooks]], and to view the actual digital sources in the authenticated environment.

- [[FALTA]] From a technical perspective, the CLARIAH Media Suite

## How has the Media Suite been built?

The overall long-term aim of the [CLARIAH Media Studies project](https://clariah.nl/en/work-packages/focus-areas/media-studies#workplan) is to build an environment that allows researchers (initially from The Netherlands) to access collections that have been unlocked for online research. CLARIAH aims to support these institutions in creating the ways to facilitate access to researchers to their collections using state-of-the art tools for searching, analysing, and combining data. The Media Suitemain guiding aim is to support the so-called "Scholarly primitives" (Unsworth, 2000), offering both to non-data expert and skillfull data-driven researchers the possibility to conduct proper research using these sources.

The Media Suite has been built as a metadata aggregator where collections can be searched and worked with simultaneously. The guiding principles for building this VRE environment are: user-friendlyness, (meta)data transparency, and triggering scholars to do data and tool criticism. 

The Media Suite has been built in two stages, based on continuous user studies and a co-development approach, which means that scholars have activelly participated in the requirement analysis, prototyping and testing faces:

- In the first stage of the CLARIAH project (from 2015 to 2017), the software engineers and developers with the input from scholars in the CLARIAH team, created the foundations of the infrastructure. The initial functional and data requirements came from prototypes created in previous projects: [[AVResearcherXL]], [[Verteld Verleden]], [[DIVE+]], [[CoMERDa]], and [[TROVe]]. 
- In the second phase, which started in April 2017, external scholars were involved as co-developers under the framework of the [[CLARIAH Research Pilot Projects]].
- This phase ended in June 2018, concluding with the launching of Version 3, where their input of these pilot projects is clearly reflected. 
- From 2018, the Media Suite will continue to be further developed in the framework of CLARIAH Plus. Future versions will focus on supporting more advanced mixed-media and audio-visual analysis methods.

> More information about how the Media Suite has been built is in our paper presented at the Digital Humanities Conference (DH2018) [Ordelman, R., Martínez Ortíz, C., Melgar Estrada, L., Koolen, M., Blom, J., Melder, W., … Noordegraaf, J. (2018). Challenges in Enabling Mixed Media Scholarly Research with Multi-media Data in a Sustainable Infrastructure – DH2018. Presented at the Digital Humanities 2018, Mexico](https://dh2018.adho.org/en/challenges-in-enabling-mixed-media-scholarly-research-with-multi-media-data-in-a-sustainable-infrastructure/).

## What are the CLARIAH Research Pilot projects?

The [CLARIAH Research pilot projects ](https://clariah.nl/projecten/research-pilots) was a grant scheme created by CLARIAH to involve researchers in the early stages of developing the Dutch Infrastructure. Six pilot projects were allocated to the Work package responsible for the Media Suite (WP5): 

- [CrossEWT](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/crossewt) ("Cross-Medial Analysis of WW2 Eyewitness Testimonies")
- [DReAM](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/dream) ("Cross media research of public debates on drugs and regulation")
- [M&M](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/m-m) ("Tracing first person in documentary history in AV-collections")
- [MIMEHIST](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/mimehist) ("Annotating EYE’s Jean Desmet Collection", focused on making available the Jean Desmet collection for film historical research)
- [NarDis](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/nardis) ("Narrativizing Disruption", focused on exploratory search in the context of using linked open data) 
- [Respons](https://clariah.nl/en/projects/research-pilots/granted-pilot-research-projects/respons) ("Remediation in Sports News").

## Where is the Media Suite hosted?

The Media Suite is hosted at the The Netherlands Institute for Sound and Vision (NISV), or (B&G), which acts as a CLARIAH centre. Not all content (media resources) are stored in this data centre though (see [[FAQ: Can I play/view all the sources that I find via the Media Suite?]].

All tools and components developed within CLARIAH are open source, the Media Suite code is available in the <a href="https://github.com/CLARIAH">CLARIAH GitHub repository page</a>. 

## Who develops the Media Suite?

The Media Suite is part of the [CLARIAH infrastructure](https://clariah.nl/en/). The CLARIAH project is divided into five workspackages. Three of the work packages specialize on developing services based on media type and for specific groups of researchers:

- WP3: Textual data (Linguistics) => [See the tools developed by WP3](https://clariah.nl/en/tools).
- WP4: Structured data (Socio-economic history) => [See the tools developed by WP4](https://clariah.nl/en/tools)
- WP5: Audio-visual data (Media studies and oral history) => Develops the Media Suite

The Media Suite is developed by one the development teams of The Netherlands Institute for Sound and Vision, part of the Research and Development department (directed by [Johan Omen](https://www.beeldengeluid.nl/en/knowledge/experts/johan-oomen)):

- [Dr. Roeland Ordelman](https://www.beeldengeluid.nl/en/knowledge/experts/roeland-ordelman): Technical coordinator of CLARIAH WP5
- [Jaap Blom](https://clariah.nl/en/about/who-is-who/wp5/jaap-blom): Head developer of the Media Suite
- [Willem Melder](https://www.beeldengeluid.nl/en/knowledge/experts/willem-melder): Data integration coordinator
- [Dr. Victor de Boer](http://www.victordeboer.com/) (linked data senior researcher and coordinator of linked data work in WP5)

- [Dr. Carlos Martínez Ortiz](https://www.esciencecenter.nl/profile/dr.-carlos-martinez-ortiz) (linked data work, collaborating software engineer from the Nederlands EScience Center)
- [Mari Wigham](https://www.linkedin.com/in/mariwigham) (data work)
- Johannes Wassenaar (data work)
- Jonathan Blok (security and authentication)
- Eduardo Navarrete (front-end support)

The development team works closely with:

- [Dr. Liliana Melgar](https://www.linkedin.com/in/lilimelgar/?locale=en_US) (requiremens analyst, researcher and tester)

- [Dr. Eva Baaren](https://www.linkedin.com/in/baaren/) (liason digital humanities)

- Scholars from WP5, lead by [Professor Julia Noordegraaf](http://www.uva.nl/profiel/n/o/j.j.noordegraaf/j.j.noordegraaf.html) (Jasmijn van Gorp, Thomas Poell, Norah Karrouche, Kaspar von Beelen), and scholars from the [[CLARIAH research pilot projects]] provide requirements, design ideas, and help in testing the Media Suite in all its phases.

The Media Suite is developed in alignment with [CLARIAH WP2](https://clariah.nl/en/work-packages/technology) (the work package responsible for the overall infrastructure coordination), and in collaboration with external partners, such as the [Netherlands EScience Center](https://www.esciencecenter.nl/), and [Frontwise](https://www.frontwise.com/).

> See Also [Wie is Wie / Who is Who in CLARIAH.
