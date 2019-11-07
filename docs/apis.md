APIs
---

The foundation of the Media Suite is built on our APIs. They facilitate the interaction with data from various collections:

- Collections API (high-level collection information (metadata: data format, size, etc.).
- Search API (searching for collection items).
- Annotation API (annotating existing data using W3C Web Annotation standard (mainly for manual annotations).
- Data Enrichment API (collection enrichment through automatic mechanisms or by human interaction).



<img src="https://github.com/CLARIAH/mediasuite-info/blob/master/docs/_images/apis.jpg?raw=true" width="700px" />



*(Figure showing the Media Suite APIs, and how they can be used via the Jupyter notebooks).*



The Data Enrichment API is not fully implemented yet (thus, it is not shown in the graphic). At this moment, it works basically in this way:

- notebook ----[create enrichment “job”]----> enrichment API
- notebook --------[get status of job]----> enrichment API
- notebook --------[get job/enrichment output]----> enrichment API
- the results of the enrichment can be put in in the annotation API, or directly in an index for the search/collection API.

*Note*: The APIs can only be used with our [Jupyter notebooks](<http://mediasuite.clariah.nl/documentation/howtos/jupyter-notebooks>) service at this moment. Please use our [Contact](http://mediasuite.clariah.nl/contact) options for more information.



   *(Last edit: November 5, 2018)* *More up to date information will be adding soon. If you have any questions, please [contact us]( https://mediasuite.clariah.nl/contact )*