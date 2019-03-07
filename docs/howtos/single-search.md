Search tool: HowTos
---

In this help menu you will learn How To:

- [Use the Search tool (Screencast)](#screencast)
- [Select collections](#data)
- [Create user projects](#user-project)
- [Use search expressions (Boolean operators)](#search-boolean)
- [Search per field (syntax)](#search-syntax)
- [Search per field (field cluster selector)](#field-cluster)
- [Filtering per date](#date-filter)
- [Understand time line charts](#timeline-charts)
- [Filter using facets](#facets)
- [Understand how search results are ranked](#result-list-ranking)
- [Order your search results](#result-list-ordering)
- [Save your query](#saved-queries)
- [Bookmark search results](#bookmarking)

---

### <a name="screencast"></a>Use the Search tool

<iframe width="560" height="315" src="https://www.youtube.com/embed/cA7c53e-MAQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>





### <a name="data"></a>Select collections

This tool uses all the data and enrichments available via the Media Suite. See [Data page](http://mediasuite.clariah.nl/data) for more information.

The Search tool works with one collection at the time, i.e., not all collections can be searched simultaneously at this moment. 

To select a collection:

1. Click on the Select collection button.
2. Observe the list of collections. You can also search collections by their title and provider, and you can read more details about each collection cliking on the "Read more" option, a separate window opens then, which brings you to the Data registry in CKAN.
3. Click on the collection you would like to use. It gets loaded and ready to use immediately by the tool.

See also other HowTos related to the inspection and understanding of the collections and data you are using:

- Inspect metadata quality
- Understand metadata (metadata dictionaries)

### <a name="user-project"></a>Create user projects

If you would like to store bookmarks and other annotations during your search, the Workspace of the Media Suite requires the creation of a User project. 

In the Search tool you can either select an existing User project or create a new one.

See also:

- What are [user projects](http://mediasuite.clariah.nl/documentation/glossary/user-project)
- [How to work with user projects](http://mediasuite.clariah.nl/documentation/workspace/user-projects)

### <a name="search-boolean"></a>Use search expressions (Boolean operators)

At this moment (version 4) the search API detects when a user does a boolean/wildcard query by looking for the keywords: 

**OR**

- Default operator. Connect two or more similar concepts (synonyms). ANY of your search terms can be present in the resulting records. Broaden your results
- Example: Koningin Beatrix 
- Searches for the word ‘Beatrix’ OR the word ‘Koningin’

**AND**

- ALL search terms must be present in the resulting records. Narrows your results
- Example1: Koningin AND Beatrix
- Example1 searches for the word ‘Koningin’ AND the word ‘Beatrix’ - but they do not have to be next to each other
- Keep into accout that the word AND has to be capitalized
- Example2: Koningin and beatrix
- Example 2 searches for items with the word ‘Koningin’ OR the word ‘and’ OR the word ‘beatrix’. 

**NOT**

- Ignore concepts (words) that may be implied by your search terms

**\***

- Wildcard which matches any character sequence (including the empty one).
- Example 1: boeren* --> boerenleven, boerenmarkt
- Example 2: boeren *  --> boeren zijn bang
- Note that a space between the last character and the asterisk wildcard influences the results

**?**

- Wildcard which matches any single character
- Example 1: vluchteling? —>  ‘vluchtelinge
- Searches for a word that starts with ‘vluchteling’ and has one extra character

**" "**

- Exact expression
- Example 1: "Broodje Aap"
- Searches for the phrase Broodje Aap

**Nesting and search order**

- Nesting queries is supported
- Use parentheses to separate the queries. The logical order in which words are connected influences the results
- Example1. (koe AND varkens) OR boeren 
- Example2. Koningin AND Beatrix NOT “Koningin Beatrix”
- Example2 searches for items with the word ‘Koningin’ AND the word ‘Beatrix’ - but NOT the phrase ‘Koningin Beatrix’. So we get e.g. items that talk about Prinses Beatrix and Koningin Juliana, but not Koningin Beatrix

**Capitalization**

- Boolean queries are not case-sensitive
- Example: bordeaux, Bourdeaux 
- Searching for any of these two terms will give the same results

**Query corrections/suggestions**

- This is not supported
- Example: koningi
- Searching for this word gives no matches (matching is precise and does not accept typos or missing letters)

Note: Future work includes supporting proximity parameters.

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

### <a name="timeline-charts"></a>Understand time line charts

(Forthcoming)

### <a name="facets"></a> Filter using facets

* Faceted search: Facets include aggregations of terms from the metadata fields of the type "Keyword field", the terms included in each facet can be used for filtering the results of your query. To see the metadata fields that are of the type "Keyword", you can use the "Inspect" tool. At this moment (version 3) we support:

  *   Default facets per collection: we include facets for the most important fields in each collection (e.g., "Broadcaster" for the Sound and Vision collection)
  *   Creation of new facets: users are allowed to add their own facets to the faceted search functionality (see screencast: Search)


### <a name="result-list-ranking"></a> Understand how search results are ranked

* List of search results: The Search tool gives a list of search results after entering your query and filters. You can in this list:

  *   Order results per relevance (description to be included soon)

  *   Order results per date: it chooses the date field you used for filtering

  *   See a summary of the metadata: using the "document" icon on the left

  *   See information per item about:

      *   Media type: there are icons on the right side of each item indicating whether it is of the type image, audio, video, or text
      *   Access: if you can "view", "play", "read" a document, you will see an icon with an open eye on the right side of the item

### <a name="result-list-ordering"></a>Order your search results

### <a name="saved-queries"></a> Save your query

* Save the query paramenters: the Search tool allows users to store the queries for further use giving them a name. See [Saved queries](http://mediasuite.clariah.nl/documentation/workspace/user-projects/queries) section for more details.

### <a name="bookmarking"></a> Bookmark search results

* After you have made a query according to your wishes using the [Search tool](http://mediasuite.clariah.nl/documentation/tools/single-search), you can select (bookmark) results to your Workspace.

* The screencast below shows how the bookmarking functionality works:

   <iframe width="560" height="315" src="https://www.youtube.com/embed/2fVNz6eh6Sg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- If you have not done so, create your own [User project](http://mediasuite.clariah.nl/documentation/workspace/user-projects) in the Work space

- Once you get a result list, use the icons on the left of the items to mark/unmark the items of your preference

- You will get a dialog window inviting you to save your bookmarks to the user project that you created in the first step

  - Note: there will be improvements in Version 4 allowing you to "remember" your selected items when changing pages in the search results. In this way, you can bookmark results across different collections during a single session.

- Another way to bookmark, individual items in this case, is via the [Resource viewer](http://mediasuite.clariah.nl/documentation/tools/resource-viewer), you will find a bookmark icon in the viewer, and also the option to select the active User project in which you want to save your bookmark.

- To see the resulting list of bookmarks, you can go to the [Workspace](http://mediasuite.clariah.nl/documentation/workspace) and find them in the User project where you have saved them. See also the [Bookmarks section](http://mediasuite.clariah.nl/documentation/workspace/user-projects/bookmarks) in the Documentation.

  

> **Please use our [Public forum](https://gitter.im/CLARIAH-media-studies/Lobby) if you miss content in this page or if you find any issues while using the Media Suite.**

*(Last update: March 7, 2019)*

