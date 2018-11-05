Tool: Search
---

Dedicated tool for searching/exploring through a single collection. 

### Data

This tool uses all the data and enrichments available via the Media Suite. See [Data page](http://mediasuite.clariah.nl/data) for more information.

### How to use

<iframe width="560" height="315" src="https://www.youtube.com/embed/cA7c53e-MAQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





Among other functionalities, it supports:

* Boolean queries: at this moment (version 3) the search API detects when a user does a boolean/wildcard query by looking for the keywords: OR, NOT, AND, * or ?

  *   Please keep into account that the default operator is OR

  *   Boolean queries are case-sensitive

  *   Nesting is supported, e.g., (koe AND varkens) OR boeren

  *   Future work includes supporting proximity parameters.

* Field cluster search: Users can determine in which group of fields they want the system to look for their query expression.

* At this moment (version 3) we support:

  *   All fields: searches in all the metadata
  *   Title field cluster: searches in all fields(per each collection) which contain titles
  *   Description field cluster: searches in all fields (per each collection) which contain descriptions (e.g., summaries, abstracts)
  *   Other clusters: depending on the collection there may be other clusters available (e.g., "Subtitles" for the Sound and Vision audio-visual collection).
  *   The list of fields that is aggregated in each cluster is included in a tool-tip
  *   Creating custom aggregations.

* Faceted search: Facets include aggregations of terms from the metadata fields of the type "Keyword field", the terms included in each facet can be used for filtering the results of your query. To see the metadata fields that are of the type "Keyword", you can use the "Inspect" tool. At this moment (version 3) we support:

  *   Default facets per collection: we include facets for the most important fields in each collection (e.g., "Broadcaster" for the Sound and Vision collection)
  *   Creation of new facets: users are allowed to add their own facets to the faceted search functionality (see screencast: Search)

* Date filters: You can limit your query to a specific period of time. It is important to keep in mind that collections often include several fields of the type "Date". To see the metadata fields that are of the type "Date", you can use the "Inspect" tool.

  *   In the date filter, you first have to select which date field you would like to use for filtering, and then enter the date range.
  *   If you don't select a date field, you won't see the visualization of your results based on time.

* List of search results: The Search tool gives a list of search results after entering your query and filters. You can in this list:

  *   Order results per relevance (description to be included soon)

  *   Order results per date: it chooses the date field you used for filtering

  *   See a summary of the metadata: using the "document" icon on the left

  *   See information per item about:

      *   Media type: there are icons on the right side of each item indicating whether it is of the type image, audio, video, or text
      *   Access: if you can "view", "play", "read" a document, you will see an icon with an open eye on the right side of the item

* Bookmark items: the screencast below shows how the bookmarking functionality works. See also the [Bookmarks section](http://mediasuite.clariah.nl/documentation/workspace/user-projects/bookmarks) in the Documentation.

  	<iframe width="560" height="315" src="https://www.youtube.com/embed/2fVNz6eh6Sg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


*(Last update: November 5, 2018)*