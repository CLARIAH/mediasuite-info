Tool: Search
---

Dedicated tool for searching/exploring through a single collection. 

### How to use

<iframe width="560" height="315" src="https://www.youtube.com/embed/cA7c53e-MAQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>



<p>Among other functionalities, it supports:</p>
<ul>
<li>
<p>Boolean queries: at this moment (version 3) the search API detects when a user does a boolean/wildcard query by looking for the keywords: OR, NOT, AND, * or ?</p>
<ul>
<li>
<p>Please keep into account that the default operator is OR</p>
</li>
<li>
<p>Boolean queries are case-sensitive</p>
</li>
<li>
<p>Nesting is supported, e.g., (koe AND varkens) OR boeren</p>
</li>
<li>
<p>Future work includes supporting proximity parameters.</p>
</li>
</ul>
</li>
<li>
<p>Field cluster search: Users can determine in which group of fields they want the system to look for their query expression.</p>
</li>
<li>
<p>At this moment (version 3) we support:</p>
<ul>
<li>All fields: searches in all the metadata</li>
<li>Title field cluster: searches in all fields(per each collection) which contain titles</li>
<li>Description field cluster: searches in all fields (per each collection) which contain descriptions (e.g., summaries, abstracts)</li>
<li>Other clusters: depending on the collection there may be other clusters available (e.g., "Subtitles" for the Sound and Vision audio-visual collection).</li>
<li>The list of fields that is aggregated in each cluster is included in a tool-tip</li>
<li>Creating custom aggregations.</li>
</ul>
</li>
<li>
<p>Faceted search: Facets include aggregations of terms from the metadata fields of the type "Keyword field", the terms included in each facet can be used for filtering the results of your query. To see the metadata fields that are of the type "Keyword", you can use the "Inspect" tool. At this moment (version 3) we support:</p>
<ul>
<li>Default facets per collection: we include facets for the most important fields in each collection (e.g., "Broadcaster" for the Sound and Vision collection)</li>
<li>Creation of new facets: users are allowed to add their own facets to the faceted search functionality (see screencast: Search)</li>
</ul>
</li>
<li>
<p>Date filters: You can limit your query to a specific period of time. It is important to keep in mind that collections often include several fields of the type "Date". To see the metadata fields that are of the type "Date", you can use the "Inspect" tool.</p>
<ul>
<li>In the date filter, you first have to select which date field you would like to use for filtering, and then enter the date range.</li>
<li>If you don't select a date field, you won't see the visualization of your results based on time.</li>
</ul>
</li>
<li>
<p>List of search results: The Search tool gives a list of search results after entering your query and filters. You can in this list:</p>
<ul>
<li>
<p>Order results per relevance (description to be included soon)</p>
</li>
<li>
<p>Order results per date: it chooses the date field you used for filtering</p>
</li>
<li>
<p>See a summary of the metadata: using the "document" icon on the left</p>
</li>
<li>
<p>See information per item about:</p>
<ul>
<li>Media type: there are icons on the right side of each item indicating whether it is of the type image, audio, video, or text</li>
<li>Access: if you can "view", "play", "read" a document, you will see an icon with an open eye on the right side of the item</li>
</ul>
</li>
</ul>
</li>
<li>
<p>Bookmark items (see the section on Workspace in this manual).</p>
</li>
</ul>
