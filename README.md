# Processing Uberon data

[![DOI: 10.5281/zenodo.45527](https://zenodo.org/badge/doi/10.5281/zenodo.45527.svg)](https://doi.org/10.5281/zenodo.45527)

[Uberon](uberon.org/ "Uberon Ontology Homepage") is "an integrated cross-species ontology … representing a variety of anatomical entities. [[source](https://doi.org/10.1186/gb-2012-13-1-r5 "Uberon, an integrative multi-species anatomy ontology")]" We [use Uberon](https://doi.org/10.15363/thinklab.d41 "Thinklab discussion") as the vocabulary to represent anatomical structures for our drug repurposing research.

## Execution

To reconstruct the analysis, run the notebooks in the following order:

1. [`human-constraint.ipynb`](human-constraint.ipynb): Compares two methods for filtering the ontology for anatomies that exist in humans.
2. [`process.ipynb`](process.ipynb): Downloads and processes the Uberon ontology in OBO format. Creates TSVs of terms, xrefs, and subsets. Additionally, creates `Uberon hetio-slim`, a subset of Uberon terms for inclusion in our hetnet.

## Datasets

The following datasets are created:

+ [`terms.tsv`](data/terms.tsv): the identifiers and names of Uberon terms
+ [`subset.tsv`](data/subset.tsv): the ontology subsets for terms
+ [`xref.tsv`](data/xref.tsv): cross-references to external vocabularies
+ [`human-constraint.tsv`](data/human-constraint.tsv): assessments of whether a term exists or not in humans based on [two methods](http://thinklab.com/d/41#12).
+ [`hetio-slim.tsv`](data/hetio-slim.tsv): the [slim term set](http://thinklab.com/d/41#16) used for our drug repurposing project.

## License

Uberon content and its derivatives are licensed under [CC-BY](http://creativecommons.org/licenses/by/3.0/ "Creative Commons Attribution 3.0 Unported"). All original content in this repository is released as [CC0](https://creativecommons.org/publicdomain/zero/1.0/ "CC0 1.0 Universal: Public Domain Dedication").
