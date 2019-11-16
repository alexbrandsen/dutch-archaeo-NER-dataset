# dutch-archaeo-NER-dataset

This repo contains a manually annotated NER dataset, consisting of Dutch archaeological excavation reports. The following entity types are labelled:

- Artefacts
- Time periods
- Materials
- Places (geographical locations)
- Archaeological contexts 
- Species

The dataset is provided in the BIO format, with each token on 1 line and empty lines denoting sentence boundaries. On each line you can find the token, PoS tag, morphological segmentation and finally the label, separated by spaces. The PoS tag and morphological segmentation are assigned by [Frog](https://languagemachines.github.io/frog/).

## Files

In the [BIO-per-file](BIO-per-file) you can find the BIO files segmented by source file. The [BIO-per-user](BIO-per-user) folder contains BIO files segmented by user. The [complete-bio-gs.bio](complete-bio-gs.bio) contains the entire dataset, and the [complete-bio-gs-with-sentence-ids-no-subPOS.bio](complete-bio-gs-with-sentence-ids-no-subPOS.bio) file also contains the entire dataset, but has added line numbers, no empty lines, and only the base PoS tag is added. This format is specifically for BERT NER scripts.

The [BIO-general-IAA](BIO-general-IAA) folder contains BIO files containing the same ~100 sentences annotated by each of the annotators, and can be used to calcuate the Inter Annotator Agreement. 

The annotation guidelines are also added (in Dutch). 

## Acknowledgements

This work was funded by a grant provided by the [Leiden Centre For Digital Humanities](https://www.universiteitleiden.nl/en/humanities/centre-for-digital-humanities)

## License

All files in this repository is licensed under a GNU GPLv3 License.

