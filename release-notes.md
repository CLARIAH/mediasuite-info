---
layout: page
title: Release notes
---
## V1 (04-01-2017)

First version of the "Recipes," "Components," "Data," and "APIs."

## V2 (12-20-2017)

Version 2 of the Media Suite has new data, bug fixes and new features. Overview:

- We added datasets/collections from The National Library of The Netherlands (KB), EYE Film Museum, and DANS.
- In the tools, we fixed a number of bugs. We also added new features that were requested by the main users (researchers).
- We implemented a “Workspace” so that you can store and retrieve your bookmarks your annotations and track your research in the Media Suite.
- We did a redesign of the interface and interaction featuring new styling and a more natural flow
- We set up the Documentation pages and blog in Github pages to facilitate later updates.

See the full list of changes below: 

**Data integration:**

- KB newspaper collection: The newspaper collection of the National Library of The Netherlands has been harvested and indexed in the Media Suite. We provide access to the data before 1945 in the first import (these data is expected to be completed to cover the entire KB dataset in the subsequent improvements of version 2).
- EYE Desmet collection: The full metadata from two of the five subsets of the EYE’s Desmet Collection have been added (i.e., the film and poster collections). Access/viewing of some of the films and posters is also possible. The two datasets have been connected when the data was available (e.g., the film records include links to the posters when these are available). Disclaimer: the date fields of the Desmet datasets from EYE include non-normalized data (e.g., 1916 (gewijzigde versie), 1912 (1911 volgens Langman). This is a normal situation in archival metdata. The cleaning of these data will be done for a subsequent release to this version. In version 2, these two datasets cannot be inspected in the Media Suite, but they can be searched and compared.
- DANS Oral history collections: The metadata from sixty four thematic collections and projects has been automatically harvested from the OAI-PMH endpoint of DANS, and indexed in the Media Suite. This does not include the speech recognition transcripts yet. Access to the content (play-out) is not possible yet.

**Major fixes and new features in the tools:**

- General improvements to the query builder: In the search and compare tools, bugs with date selections have been solved, time slider for selecting dates has been changed to date picker, Boolean queries are enabled, field clusters to the Sound and Vision Collection have been added.
- General improvements to the results and result list: In the search and compare tools issues with display of titles and dates have been solved, basic statistics of results per collection have been added, tooltips have been included, the resource viewer has been splitted into summary view and detailed view.
- General improvements to the graphics/visualizations: The main bugs and issues with timeline chart and histogram in the Collection Inspector and Search and Compare tools have been solved. The dynamics of the time-line chart has been improved, the histogram is located in a more visible place, absolute values from results in a given point of time have been added to the graphics.
- Fixes and new features in the Collection inspector tool: Bugs in the calculations have been fixed, statistics presentation has been made more transparent, issues with dates in the date field axis of the timeline chart have been fixed, the syntax and grouping of the metadata fields and their types has been made more user-friendly, a search box for metadata fields has been added for string search.
- Fixes and new features in the Search tool: Collections can be added directly from this tool.
- Improvements to the annotation tool: Display of titles for segments has been improved, new option to add custom links.
- Fixes and new features in the Exploratory browser: The four datasets (Tropenmuseum, KB news bulletins, Amsterdam Museum and OpenImages) in the new version remain unchanged with respect to previous versions of the exploratory browser. Changes include updated event labels for the news bulletins, based on extraction work by Kim Bosman. Additional events have been extracted for the Tropenmuseum data based on work by Victor Kramer. Furthermore, provenance and license information has been added for media objects as well as for metadata triples (named graphs). Filtering in the DIVE browser has been improved. Note: the integration of this browser in the linked data/tools workflow of the Media Suite will be included in Version 3 and 4.

**NEW! Workspace**

- Option to create user projects: You can create your own projects and store bookmarks, annotations, and search sessions. These projects can be private or public (other users can see the data stored by the individual users in a project)
- Bookmarking resources and adding them to projects: Each individual result can be bookmarked and added to a user project from the resource viewer.
- Saving tool sessions: We are working on a feature that enables you to store a tool session, including its queries and filter settings. The Media Suite is already able to display this data.
- Implementing this feature in the tools is planned for next year. Currently there is an example DIVE+ tool session, that demonstrates this feature.
- Viewing user projects: All user projects per user, and public projects can be viewed in a list, opened, and exported.
- Viewing user bookmarks and annotations: All aggregated bookmarks and annotations added by a user can be viewed in two ways: a list of bookmarks with annotations, or a list of aggregated annotations with links to the items they correspond to.
- Exporting user projects, bookmarks and annotations: All data in the work space can be exported to a JSON file.

**Major styling and design**
During the last three months of 2017 we worked on improving the styling of the Media Suite user interface and the design of the workspace. This resulted in a new design, that includes:

- Inclusion of (styled) new features that support scholars in all research phases, including brand new Workspace features!
- Improved user flow that supports easy navigation between Data, Tools and Workspace.
- Consistent styling that makes the UI more user friendly and gives it a recognizable and professional look and feel.

**A lot of invisible/back-end work:**
The development team made significant progress in building the Media Suite with an infrastructural approach, this means that there has been a lot of effort put into servers’ maintenance, such as: the semi-automatic process for the deployment of the entire infrastructure (for both a test and production environment), versioning control, backups of data & virtual servers; a scaled up data cluster; security of APIs & video play-out; enhancements of the annotation model & functionalities are amongst many others...

**Note**: Release of Version 3 is planned for April 2018 with possibly some smaller updates in between.

## V2.1 (01-25-2018)

This version has improved bookmarking functionalities and more:

- We added functionality for bookmarking multiple search results from the single search page
- You can now organize your bookmarks by arranging them in different lists within your project (viewable in your workspace)
- Each search result now includes media type & accessibility information
- The Beeld en Geluid collection by default now shows much more genres in the "genre facet", since it is now tied to the "series level" metadata, instead of the "program level" metadata
- Miscellaneous small updates to the user interface

## V3 (20-06-2018)

Version 3 of the Media Suite has new data, bug fixes and many new features!:

- A significant portion of the collections of The Netherlands Institute for Sound and Vision has gone through automatic speech recognition processes (ASR), resulting in transcripts available for search and interactive navigation of the resources. The process is still ongoing. In Version 3 transcripts are available for:

  - Radio 1 (Hilversum 1, NPO Radio 1): more than 90%
  - Radio 5 (747 AM, NPO Radio 5): more than 60%
  - Source catalogs (items from the Radio Programma, Weken Nederlandse Radio, and Hoorspelen  collections): more than 40%
  - Television (news and current affairs): about 25%

- We added new collections and increased access to resources from collections from EYE Film Museum (this is the result of a collaborative effort between the researchers of the [MIMEHIST research pilot project](https://clariah.nl/projecten/research-pilots/mimehist), the development team of the Media Suite, the curators at EYE, and [CREATE](http://www.create.humanities.uva.nl/) at the University of Amsterdam:

  - The Jean Desmet business archive has been made fully available for browsing (according to the same archival structure provided by EYE).

  - The Desmet business archive can also be searched, thanks to experiments with OCR-ing this collection by Ivan Kisjes from the CREATE program. The OCR allows for searching the full text of the typed written documents. Other automatic detection experiments allow to group items per type (e.g., letters, telegrams, etc.), logos, signatures, languages, among others.  "[^1]

    [^1]: >For more detailed information about these experiments  Kisjes, I., & Olesen, C. (2018). OCR’ing and classifying Jean Desmet’s business archive: methodological implications and new directions for media historical research – DH2018. Presented at the Digital Humanities 2018. Retrieved from <https://dh2018.adho.org/en/ocring-and-classifying-jean-desmets-business-archive-methodological-implications-and-new-directions-for-media-historical-research/>.

  - Viewing of the more than one hundred thousand digitized images is possible via a IIIF server. 

  - Those images can be annotated.

  - The Desmet film collection, which metadata was made available in Version 2 of the Media Suite linking to the publicly accessible Youtube videos, is now fully available for viewing, more than eight hundred films can be played from the EYE servers via the Media Suite!

- The "open/open access" oral history interviews at DANS can be now played and annotated via the Media Suite.

- There were improvements to the data completeness of The Netherlands Institute of Sound and Vision after detailed data integrity checks.

- The Inspector tool has been redesigned and improved with "[[metadata dictionaries]]".

- We redesigned the Compare tool to work with the newly implemented [[Saved queries]]. 

- We fixed a number of bugs in the Search tool. We also added new features that were requested by the main users (researchers) to all tools. These include:

  - Improved faceted search
  - Saved queries!
  - Improvements to the timeline charts and histograms
  - Improvements to the Bookmarking facilities

- In the browsing tool ("Explore") we made possible to connect the resources to the Workspace functionalities. Users can now add bookmarks and annotate resources from the Explore tool, save "Tool sessions," and find all these in their Workspace.

- The browsing tool ("Explore"), new functionalities were added to facilitate adding comments to [[Browsing paths]]

- We improved significantly the “Workspace,” which first version was launched in the previous release of the Media Suite:

  - All views (bookmarks, codes, comments, links, metadata cards) were split for improving clarity
  - Each view was improved with filtering options
  - Viewing and exporting user fragments became more clear 

- We improved interface and interaction.

- The Documentation pages and blog in Github pages have been fully updated.
