## Tool: Inspect

This is a tool for the inspection of the metadata types in a collection, as well as for the evaluation of metadata quality of those fields. At this moment (Version 3), the Inspect tool offers the option to evaluate metadata completeness, which is calculated based on the number of records for which a given metadata field has been filled in. This completeness can be evaluated per field (all years), or along time. 

### Background

The "collection inspection" functionalities support the scholarly tasks of *data criticism* by facilitating the close inspection of the metadata fields that constitute each collection. 

The purpose of this tool is to provide an overview of how a collection/dataset is constituted and also to allow a closer inspection of their metadata (e.g., detect incomplete data, or observe value distributions along date fields). 

It is important to have clear that the collection inspector does not give search results. Future developments include the integration of other metrics (besides completeness) for the evaluation of metadata quality, and the possibility to visualize metadata completeness together with search results. 

### How to use

1. When you open the Inspect tool you will find a button to add a Collection. This opens the "Collection selector," where you can see the available collections (see [FAQ section: What kind of data is available via the Media Suite?](http://mediasuite.clariah.nl/documentation/faq/what-data))
2. When you select a collection, you can inspect its metadata fields by clicking on "Select field to analyse"
3. In this graphic you can see the completeness of ONE metadata field over time. The timeline chart uses a date field selected by the user. Be aware that these date fields are also metadata, and that they can also be more or less complete. You can evaluate the completeness of a date field as well, using the first option in Step 1.
4. There is a [Jupyter notebook](http://mediasuite.clariah.nl/documentation/workspace/jupyter-notebooks) prepared for complementing the functions available in this tool. For example:
   - If you want to compare the completeness of two or more metadata fields
   - If you want to check the metadata completeness of a section of the collection (e.g., for resources of a certain media type)

   > If you are interested in the completeness of the ASR (automatic speech recognition transcripts) of the Netherlands Institute for Sound and Vision's audio-visual collection, visit [this page](http://mediasuite.clariah.nl/documentation/data/automatic-enrichments).