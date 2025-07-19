# [Adapting Multilingual Embedding Models to Historical Luxembourgish](https://www.arxiv.org/abs/2502.07938) Reproduction code, models and datasets
![License: AGPLV3+](https://img.shields.io/badge/License-AGPLV3+-brightgreen.svg)


## Overview

This repository allows replication of the experiments from the research titled "Adapting Multilingual Embedding Models to Historical Luxembourgish". This repository includes:

- Scripts and notebooks to replicate the training and evaluation of the examined models.
- The training and test data created through articles in Historical Luxembourgish.
- Our reccomended adapted models to be used for semantic search to and from Historical Luxembourgish.

## Repository Organization:

The repository is organized as follows:

```
├── RAW_test_set_sentences
│   └── The test set sentences that constitute the bitext mining task, in a jsonl raw unprocessed format.
├── prepared_training_sentences
│   └── The prepared sentences pairs used within the training set. (Also available in HuggingFace datasets format)
├── raw_translations_json
│   └── The original post-corrected translations files before training and test split.
├── HistLuxEmb_Prepare_Data_and_Evaluation.ipynb
│   └── Jupyter notebook to follow through to prepare the data (including utilities) and evaluate existing models.
├── HistLuxEmb_Contrastive_Training.ipynb
│   └── Jupyter notebook to follow through to perform the contrastive training that was appleid to LaBSE, LuxEmbedder and M-GTE.
├── HistLuxEmb_M-Mpnet_Knowledge_Dist.py
│   └── Python script to extend the Multilingual-MPNet model to support Historical and Modern Luxembourgish.
```

## Released Datasets:

Training Set:

[HistLuxAlign](https://huggingface.co/datasets/impresso-project/HistLuxAlign)

Bitext Mining Test Set (already prepared for convenience):

[GoogleDriveLink](https://drive.google.com/file/d/1B_na_iXXa5nNcfh8L7sNIln9hNkji0ad/view?usp=share_link)

## Released Models:

Reccomended: [histlux-gte-multilingual-base](https://huggingface.co/impresso-project/histlux-gte-multilingual-base)

Alternative: [histlux-paraphrase-multilingual-mpnet-base-v2](https://huggingface.co/impresso-project/histlux-paraphrase-multilingual-mpnet-base-v2)

## Further Support
If you are interested in contributing or need further support reproducing/recreating/extending the results, please reach out to andrianos.michail@cl.uzh.ch.

## BibTeX Reference

If you would like to cite this project, or the associated paper, here's a bibtex:

```bibtex
@inproceedings{michail-etal-2025-adapting,
    title = "Adapting Multilingual Embedding Models to Historical {L}uxembourgish",
    author = "Michail, Andrianos  and
      Racl{\'e}, Corina  and
      Opitz, Juri  and
      Clematide, Simon",
    editor = "Kazantseva, Anna  and
      Szpakowicz, Stan  and
      Degaetano-Ortlieb, Stefania  and
      Bizzoni, Yuri  and
      Pagel, Janis",
    booktitle = "Proceedings of the 9th Joint SIGHUM Workshop on Computational Linguistics for Cultural Heritage, Social Sciences, Humanities and Literature (LaTeCH-CLfL 2025)",
    month = may,
    year = "2025",
    address = "Albuquerque, New Mexico",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.latechclfl-1.26/",
    doi = "10.18653/v1/2025.latechclfl-1.26",
    pages = "291--298",
    ISBN = "979-8-89176-241-1",
}
```

## About Impresso

### Impresso project

[Impresso - Media Monitoring of the Past](https://impresso-project.ch) is an interdisciplinary research project that aims to develop and consolidate tools for processing and exploring large collections of media archives across modalities, time, languages and national borders. The first project (2017-2021) was funded by the Swiss National Science Foundation under grant No. [CRSII5_173719](http://p3.snf.ch/project-173719) and the second project (2023-2027) by the SNSF under grant No. [CRSII5_213585](https://data.snf.ch/grants/grant/213585) and the Luxembourg National Research Fund under grant No. 17498891.

### Copyright

Copyright (C) 2025 The Impresso team.

### License

This program is provided as open source under the [GNU Affero General Public License](https://github.com/impresso/impresso-pyindexation/blob/master/LICENSE) v3 or later.

<p align="center">
  <img src="https://github.com/impresso/impresso.github.io/blob/master/assets/images/3x1--Yellow-Impresso-Black-on-White--transparent.png?raw=true" width="350" alt="Impresso Project Logo"/>
</p>
