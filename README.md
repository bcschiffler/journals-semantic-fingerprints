# Semantic fingerprinting of scientific journals

To compare the similarity of texts, it is helpful to get an aggregate representation of the relevant texts. The notebook in this repo displays the semantic overlap in content between major scientific journals in the biomedical field.

We are going to be using the [cortical.io](http://cortical.io) API to get a semantic fingerprint for the abstracts from every journal, compare them using the [Jaccard distance metric](https://en.wikipedia.org/wiki/Jaccard_index) and finally plot them in an interactive map using [Bokeh](https://bokeh.pydata.org/en/latest).

Semantic fingerprinting is a technique based on embedding a word or text in a context so that the conceptual links to other concepts are being revealed. There are many ways to embed a text in a vector space. The method I am showing in this notebook relies on [semantic folding](https://en.wikipedia.org/wiki/Semantic_folding). It has its origins in theoretical concepts on how the brain could be storing information, e.g., theories about [sparse distributed representations](https://arxiv.org/ftp/arxiv/papers/1503/1503.07469.pdf).
Find more information about semantic fingerprinting [here](http://www.cortical.io/technology_semantic.html).

The data used in this notebook (a sample of 200 abstracts for each journal) stems from Pubmed queries and can e.g., be obtained using the scripts in [this repository](https://github.com/wiheto/readabilityinscience). However, with adjustments it can be used to gather semantic fingerprints and compare them for any text-based data.

The final output html file is hosted [here](http://bcschiffler.com/journals_200.html).
