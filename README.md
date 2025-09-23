<h2 align="center">🚧 <b>This project is continuously updating. Please check back soon!</b> 🚧</h2>



# SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)


This is the official repository for the dataset and code of the paper:  ["SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP"](https://arxiv.org/abs/2509.07801),  *accepted at **EMNLP 2025** (Main Conference)*.


## 📚 SciNLP

Our dataset is constructed based on resources from [The ACL OCL Corpus](https://github.com/shauryr/ACL-anthology-corpus) (Shaurya Rohatgi, 2022) . 
The dataset can be accessed at:  [SciNLP](https://github.com/AKADDC/SciNLP)  

It contains four files:  

- **train/test/dev.json**: Train, dev and test data set of SciNLP data set.  
- **KG_triples.txt**: Triples extracted from [the ACL Anthology](https://aclanthology.org/) PDFs by using the [HGERE](https://github.com/yanzhh/HGERE) model based on SciNLP training

### Data format

The data format for models is JSON. Each line of the input file contains one document in the following format.

```
{
  # document ID (please make sure doc_key can be used to identify a certain document)
  "doc_key": "2020.acl-main.21",

  # sentences in the document, each sentence is a list of tokens
  "sentences": [
    [...],
    [...],
    ["Prior", "works", "performed", "SQG", "on", "CoQA", ...],
    ...
  ],

  # entities (boundaries and entity type) in each sentence
  "ner": [
    [...],
    [...],
    [[3, 3, "task"], [5, 5, "dataset"], ...], #the boundary positions are indexed in the document level
    ...,
  ],

  # relations (two spans and relation type) in each sentence
  "relations": [
    [...],
    [...],
    [[3, 3, 5, 5, "evaluatedOn"] ...],
    ...
  ]
}
```

## 💻 Code for LLMs-Baselines

Our used supervised methods include:

- [PURE](https://github.com/princeton-nlp/PURE)
- [PL-Marker](https://github.com/thunlp/PL-Marker)
- [HGERE](https://github.com/yanzhh/HGERE)


## 📜 License

SciNLP is released under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/legalcode) license.  The dataset follows the same policy as [The ACL OCL Corpus](https://allenai.org/data/s2orc) : **for non-commercial academic research use only**.


## 📖 References

If you use this dataset, please cite the following works:

```bibtex

@inproceedings{scinlp,
  author    = {Decheng Duan, Yingyi Zhang, Jitong Peng and Chengzhi Zhang},
  title     = {SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP},
  booktitle = {Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP2025)},
  year      = {2025},
  address   = {Suzhou, China}
}

@Misc{acl_anthology_corpus,
    author =       {Shaurya Rohatgi},
    title =        {ACL Anthology Corpus with Full Text},
    howpublished = {Github},
    year =         {2022},
    url =          {https://github.com/shauryr/ACL-anthology-corpus}
}

