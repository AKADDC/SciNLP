<h2 align="center">🚧 <b>This project is continuously updating. Please check back soon!</b> 🚧</h2>



# SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP



This is the official repository for the dataset and code of the paper:  ["SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP"](),  *accepted at **EMNLP 2025** (Main Conference)*.


## 📚 SciNLP

Our dataset is constructed based on resources from [The ACL OCL Corpus](https://github.com/shauryr/ACL-anthology-corpus) (Shaurya Rohatgi, 2022) . 
The dataset can be accessed at:  [SciNLP](https://github.com/AKADDC/SciNLP)  

It contains four files:  

- **train/test/dev.json**: Train, dev and test data set of SciNLP data set.  
- **KG_triple.txt**: Triples extracted from HGERE model based on SciNLP training

## 🛠️ Preparation Before Starting

Before using the SurveyGen framework, please ensure you have the following resources ready:

3. **LLM API access** — Apply for access to the LLMs or deploy the LLMs locally.  

## 💻 Code for LLMs-Baselines


## 📜 License

SciNLP is released under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/legalcode) license.  The dataset follows the same policy as [The ACL OCL Corpus](https://allenai.org/data/s2orc) : **for non-commercial academic research use only**.


## 📖 References

If you use this dataset, please cite the following works:

```bibtex

@inproceedings{scinlp,
  author    = {Decheng Duan and Yingyi Zhang Nayeem and Jitong Peng and Chengzhi Zhang},
  title     = {SciNLP: A Domain-Specific Benchmark for Full-Text Scientific Entity and Relation Extraction in NLP},
  booktitle = {Proceedings of the 2025 Conference on Empirical Methods in Natural Language Processing (EMNLP)},
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

