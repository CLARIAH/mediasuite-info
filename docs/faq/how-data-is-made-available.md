## How does the Media Suite make the data available?

Technically, the integration of the metadata into the Media Suite is done either:

1. By using the [[APIs]] of the content providers (when available)
2. By harvesting the metadata exposed via [[OAI-PMH]] protocols (when available), or,
3. Via [[data dumps]].

Accessing the media resources (videos, audio, images, text) works in a different way. In most cases, these objects are hosted by the[ contributing institutions or projects](http://mediasuitedata.clariah.nl/group), and the Media Suite provides access to "playout" or "viewing" functionality either inside the [[Resource viewer]], or by redirecting the users to the original provider (this is done, for example, in the case of the KB newspaper collection).

Since one of the aims of CLARIAH is to encourage and support institutions to make their data available to researchers, in any of these cases, data provision is done in collaboration between CLARIAH and the[ contributing memory institutions or projects](http://mediasuitedata.clariah.nl/group). Developers, scholars, and the curators from the institutions providing these data to be accessed via the CLARIAH Media Suite have been working together to make collections available via the Media Suite.

From the technical perspective, the Media Suite works with documents expressed in [[JSON]] format. These documents are stored in [[ElasticSearch]] (ES) indexes, which can be search and retrieved using Lucene (a free and open source information retrieval software library). The strengths of ES are the support to faceted search and full text retrieval.

In parallel, there is ongoing work in converting all collections available via the Media Suite to JSON-LD documents (linked open data). This is with the aim to facilitate future integration with ANANSI [[Data]], the CLARIAH linked data central connection of all datasets. In version 3, the Media Suite offers only one experimental collection in JSON-LD (Open Images from The Netherlands Institute for Sound and Vision). This collection can be browsed using the [[Exploratory search tool]]. The “media objects” available in this way, are connected to the ES indexes, thus, users can seamlessly search and navigate this collection in both the ES-based Media Suite tools and the linked-data based exploratory tool.