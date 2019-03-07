Tool: Search
---

Dedicated tool for searching/exploring through a single collection. In this help menu you will learn:

- [How to use this tool (Screencast)](#screencast)
- [Data used by this tool](#data)
- [Search expressions (Boolean operators)](#search-boolean)
- [Search per field (syntax)](#search-syntax)
- [Search per field (field cluster selector)](#field-cluster)
- [Filtering per date](#date-filter)
- [Time line charts](#timeline-charts)
- [Filtering using facets](#facets)
- [Search results (ranking, ordering)](#result-list)
- [Save query](#saved-queries)
- [Bookmarking search results](#bookmarking)

---

### <a name="screencast"></a> How to use this tool

<iframe width="560" height="315" src="https://www.youtube.com/embed/cA7c53e-MAQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





### <a name="data"></a> Data used by this tool

This tool uses all the data and enrichments available via the Media Suite. See [Data page](http://mediasuite.clariah.nl/data) for more information.

### <a name="search-boolean"></a> Search expressions (Boolean operators)

- At this moment (version 4) the search API detects when a user does a boolean/wildcard query by looking for the keywords: 

  ```
  
  ```

  ​	, 

  ​	**NOT** 

  ​	**AND** 

  ​	***** (). Example: it should be boeren* 	and not boeren *

  ​	**?** (wildcard which matches any single character, e.g., if you search for <u>migra?t</u>, you will find matches 	with terms such as: <u>migranten</u>, <u>migrantenvoorganger</u>, among others)

*   Boolean queries are case-sensitive

*   Nesting is supported, e.g., (koe AND varkens) OR boeren

*   Future work includes supporting proximity parameters.

### <a name="search-syntax"></a> Search per field (syntax)

(Forthcoming)

### <a name="field-cluster"></a> Search per field (field cluster selector)

Users can determine in which group of fields they want the system to look for their query expression.

* At this moment (version 4) we support:

  *   All fields: searches in all the metadata
  *   Title field cluster: searches in all fields(per each collection) which contain titles
  *   Description field cluster: searches in all fields (per each collection) which contain descriptions (e.g., summaries, abstracts)
  *   Other clusters: depending on the collection there may be other clusters available (e.g., "Subtitles" for the Sound and Vision audio-visual collection).
  *   The list of fields that is aggregated in each cluster is included in a tool-tip
  *   Creating custom aggregations.


### <a name="date-filter"></a> Filtering per date

You can limit your query to a specific period of time. It is important to keep in mind that collections often include several fields of the type "Date". To see the metadata fields that are of the type "Date", you can use the "Inspect" tool and consult the metadata dictionaries.

- In the date filter, you first have to select which date field you would like to use for filtering, and then enter the date range. For example, for The Sound and Vision audiovisual collection, we recommend to select the field "programsortdate (in: publications)" (which is the equivalent to the "broadcasting date"). You can check how complete this metadata field has been over time by using the Inspector tool.
- If you don't select a date field, you won't see the visualization of your results based on time.

### <a name="timeline-charts"></a> Time line charts

(Forthcoming)

### <a name="facets"></a> Filtering using facets

* Faceted search: Facets include aggregations of terms from the metadata fields of the type "Keyword field", the terms included in each facet can be used for filtering the results of your query. To see the metadata fields that are of the type "Keyword", you can use the "Inspect" tool. At this moment (version 3) we support:

  *   Default facets per collection: we include facets for the most important fields in each collection (e.g., "Broadcaster" for the Sound and Vision collection)
  *   Creation of new facets: users are allowed to add their own facets to the faceted search functionality (see screencast: Search)


### <a name="result-list"></a> Search results (ranking, ordering)

* List of search results: The Search tool gives a list of search results after entering your query and filters. You can in this list:

  *   Order results per relevance (description to be included soon)

  *   Order results per date: it chooses the date field you used for filtering

  *   See a summary of the metadata: using the "document" icon on the left

  *   See information per item about:

      *   Media type: there are icons on the right side of each item indicating whether it is of the type image, audio, video, or text
      *   Access: if you can "view", "play", "read" a document, you will see an icon with an open eye on the right side of the item

### <a name="saved-queries"></a> Save query

* Save the query paramenters: the Search tool allows users to store the queries for further use giving them a name. See [Saved queries](http://mediasuite.clariah.nl/documentation/workspace/user-projects/queries) section for more details.

### <a name="bookmarking"></a> Bookmarking search results

* Bookmark items: the screencast below shows how the bookmarking functionality works. See also the [Bookmarks section](http://mediasuite.clariah.nl/documentation/workspace/user-projects/bookmarks) in the Documentation.

   <iframe width="560" height="315" src="https://www.youtube.com/embed/2fVNz6eh6Sg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



> **Please use our [Public forum](https://gitter.im/CLARIAH-media-studies/Lobby) if you miss content in this page or if you find any issues while using the Media Suite.**

*(Last update: January 29, 2019)*

