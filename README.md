# Awesome-LLM-Tabular
[![Awesome](https://awesome.re/badge.svg)](https://github.com/johnnyhwu/Awesome-LLM-Tabular)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

![](/resource/other/banner.png)

:bulb: Since the emergence of ChatGPT, Large Language Models (LLMs) have garnered significant attention, with new advancements continuously emerging. LLMs have found applications in various domains like vision, audio, and text tasks. However, **tabular data** remains a crucial data format in this world. Hence, this repo focuses on collecting research papers that explore the integration of LLM technology with tabular data, and aims to save you valuable time and boost research efficiency.

:sparkles: Awesome-LLM-Tabular is a curated list of **Large Language Model** applied to **Tabular Data**.

:fire: This project is currently under development. Feel free to :star: (STAR) and :telescope: (WATCH) it to stay updated on the latest developments.

## Table of Content

- [Awesome-LLM-Tabular](#awesome-llm-tabular)
  - [Table of Content](#table-of-content)
  - [Related Papers](#related-papers)
  - [Workshops](#workshops)
  - [Useful Blogs](#useful-blogs)

## Related Papers

| Date | keywords | Paper | Publication | Resource |
| :--: | :------: | :---: | :---------: | :------: |
| 2019/09 | TabFact | [TabFact: A Large-scale Dataset for Table-based Fact Verification](https://arxiv.org/abs/1909.02164) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/wenhuchen/Table-Fact-Checking?tab=readme-ov-file) |
| 2020 | TableGPT | [TableGPT: Few-shot Table-to-Text Generation with Table Structure Reconstruction and Content Matching](https://aclanthology.org/2020.coling-main.179.pdf) | ![Static Badge](https://badgen.net/badge/color/COLING/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/syw1996/TableGPT) |
| 2020/05 | TaBERT | [TaBERT: Pretraining for Joint Understanding of Textual and Tabular Data](https://arxiv.org/abs/2005.08314) | ![Static Badge](https://badgen.net/badge/color/ACL/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/facebookresearch/TaBERT) |
| 2020/09 | GaPPa | [GraPPa: Grammar-Augmented Pre-Training for Table Semantic Parsing](https://arxiv.org/abs/2009.13845) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/taoyds/grappa) |
| 2022/02 | TableQuery | [TableQuery: Querying tabular data with natural language](https://arxiv.org/pdf/2202.00454.pdf) | | |
| 2022/05 | FeSTE      | [Few-Shot Tabular Data Enrichment Using Fine-Tuned Transformer Architectures](https://aclanthology.org/2022.acl-long.111.pdf) | ![Static Badge](https://badgen.net/badge/color/ACL/blue?label=) | |
| 2022/05 | FM        | [Can Foundation Models Wrangle Your Data?](https://arxiv.org/abs/2205.09911) | ![Static Badge](https://badgen.net/badge/color/VLDB/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/HazyResearch/fm_data_tasks) |
| 2022/05 | TURL | [Technical Perspective of TURL: Table Understanding through Representation Learning](https://dl.acm.org/doi/abs/10.1145/3542700.3542708) | ![Static Badge](https://badgen.net/badge/color/SIGMOD/blue?label=) | |
| 2022/06 | TabText    | [TabText: A Flexible and Contextual Approach to Tabular Data Representation](https://arxiv.org/abs/2206.10381) | | |
| 2022/06 | LIFT       | [LIFT: Language-Interfaced Fine-Tuning for Non-Language Machine Learning Tasks](https://arxiv.org/abs/2206.06565) | ![Static Badge](https://badgen.net/badge/color/NeurIPS/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/UW-Madison-Lee-Lab/LanguageInterfacedFineTuning) |
| 2022/09 | PTab | [PTab: Using the Pre-trained Language Model for Modeling Tabular Data](https://arxiv.org/pdf/2209.08060.pdf) | | |
| 2022/09 | TabMWP | [Dynamic Prompt Learning via Policy Gradient for Semi-structured Mathematical Reasoning](https://arxiv.org/abs/2209.14610) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://promptpg.github.io/) |
| 2022/10 | GReaT | [Language Models are Realistic Tabular Data Generators](https://arxiv.org/pdf/2210.06280.pdf) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/kathrinse/be_great) |
| 2022/10 | TabLLM | [TabLLM: Few-shot Classification of Tabular Data with Large Language Models](https://arxiv.org/pdf/2210.10723.pdf) | ![Static Badge](https://badgen.net/badge/color/AISTATS/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/clinicalml/TabLLM) |
| 2023/?? | IngesTables | [IngesTables: Scalable and Efficient Training of LLM-Enabled Tabular Foundation Models](https://openreview.net/pdf?id=EocsZtcA7P) | ![Static Badge](https://badgen.net/badge/color/TRL@NeurIPS/blue?label=) | |
| 2023/?? | Elephants | [Elephants Never Forget: Testing Language Models for Memorization of Tabular Data](https://arxiv.org/abs/2403.06644) | ![Static Badge](https://badgen.net/badge/color/TRL@NeurIPS/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/interpretml/LLM-Tabular-Memorization-Checker) |
| 2023/01 | DATER | [Large Language Models are Versatile Decomposers: Decompose Evidence and Questions for Table-based Reasoning](https://arxiv.org/abs/2301.13808) | ![Static Badge](https://badgen.net/badge/color/SIGIR/blue?label=) | |
| 2023/02 | AdaPTGen | [Adapting Prompt for Few-shot Table-to-Text Generation](https://arxiv.org/abs/2302.12468) | | |
| 2023/03 | Survey Paper | [Transformers for Tabular Data Representation: A Survey of Models and Applications](https://aclanthology.org/2023.tacl-1.14/) | ![Static Badge](https://badgen.net/badge/color/TACL/blue?label=) | |
| 2023/04 | TABLET | [TABLET: Learning From Instructions For Tabular Data](https://arxiv.org/pdf/2304.13188.pdf) | | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/dylan-slack/Tablet) |
| 2023/05 | AnyPredict | [AnyPredict: Foundation Model for Tabular Prediction](https://arxiv.org/pdf/2305.12081.pdf) | | |
| 2023/05 | TAPTAP | [Generative Table Pre-training Empowers Models for Tabular Prediction](https://arxiv.org/abs/2305.09696) | ![Static Badge](https://badgen.net/badge/color/ACL/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/ZhangTP1996/TapTap) |
| 2023/07 | TableGPT | [TableGPT: Towards Unifying Tables, Nature Language and Commands into One GPT](https://arxiv.org/pdf/2307.08674.pdf) | | |
| 2023/07 | UniTabE | [UniTabE: A Universal Pretraining Protocol for Tabular Foundation Model in Data Science](https://arxiv.org/abs/2307.09249) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | |
| 2023/10 | TabFMs | [TOWARDS FOUNDATION MODELS FOR LEARNING ON TABULAR DATA](https://arxiv.org/pdf/2310.07338.pdf) | | |
| 2023/10 | TableFormat | [Tabular Representation, Noisy Operators, and Impacts on Table Structure Understanding Tasks in LLMs](https://arxiv.org/abs/2310.10358) | | |
| 2023/10 | UniPredict | [UniPredict: Large Language Models are Universal Tabular Classifiers](https://arxiv.org/abs/2310.03266) | | |
| 2023/10 | Table-GPT | [Table-GPT: Table-tuned GPT for Diverse Table Tasks](https://arxiv.org/abs/2310.09263) | |  [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/microsoft/Table-GPT) |
| 2024/03 | TableLLM | [Table Meets LLM: Can Large Language Models Understand Structured Table Data? A Benchmark and Empirical Study](https://dl.acm.org/doi/abs/10.1145/3616855.3635752) | ![Static Badge](https://badgen.net/badge/color/WSDM/blue?label=) | |
| 2023/11 | NumericalReasoning | [Exploring the Numerical Reasoning Capabilities of Language Models: A Comprehensive Analysis on Tabular Data](https://arxiv.org/abs/2311.02216) | ![Static Badge](https://badgen.net/badge/color/EMNLP/blue?label=) | |
| 2023/12 | TaCo | [Chain-of-Thought Reasoning in Tabular Language Models](https://aclanthology.org/2023.findings-emnlp.734/) | ![Static Badge](https://badgen.net/badge/color/EMNLP/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/SpursGoZmy/TaCo) |
| 2024/01 | Chain-of-Table | [Chain-of-Table: Evolving Tables in the Reasoning Chain for Table Understanding](https://arxiv.org/abs/2401.04398) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | |
| 2024/01 | TAT-LLM | [TAT-LLM: A Specialized Language Model for Discrete Reasoning over Tabular and Textual Data](https://arxiv.org/abs/2401.13223) | | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://huggingface.co/next-tat) |
| 2024/02 | Survey Paper | [LLM on Tabular Data: Prediction, Generation, and Understanding](https://arxiv.org/abs/2402.17944) | | |
| 2024/02 | CABINET | [CABINET: Content Relevance based Noise Reduction for Table Question Answering](https://arxiv.org/abs/2402.01155) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/Sohanpatnaik106/CABINET_QA) |
| 2024/02 | OpenTab | [OpenTab: Advancing Large Language Models as Open-domain Table Reasoners](https://arxiv.org/abs/2402.14361) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/Sohanpatnaik106/CABINET_QA) |
| 2024/02 | CancerGPT | [CancerGPT for few shot drug pair synergy prediction using large pretrained language models](https://www.nature.com/articles/s41746-024-01024-9) | ![Static Badge](https://badgen.net/badge/color/Nature/blue?label=) | |
| 2024/02 | Exploration of LLM on Tabular | [Tables as Images? Exploring the Strengths and Limitations of LLMs on Multimodal Representations of Tabular Data](https://arxiv.org/html/2402.12424v3) | | |
| 2024/03 | TableLLM | [Table Meets LLM: Can Large Language Models Understand Structured Table Data? A Benchmark and Empirical Study](https://dl.acm.org/doi/abs/10.1145/3616855.3635752) | ![Static Badge](https://badgen.net/badge/color/WSDM/blue?label=) | |
| 2024/03 | ITAB-LLM | [Unleashing the Potential of Large Language Models for Predictive Tabular Tasks in Data Science](https://arxiv.org/abs/2403.20208) | | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://huggingface.co/OldBirdAZ/itab-llm) |
| 2024/03 | TP-BERTa | [Making Pre-trained Language Models Great on Tabular Prediction](https://arxiv.org/abs/2403.01841) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/jyansir/tp-berta) |
| 2024/04 | FeatLLM | [Large Language Models Can Automatically Engineer Features for Few-Shot Tabular Learning](https://arxiv.org/pdf/2404.09491.pdf) |  | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/Sungwon-Han/FeatLLM) |
| 2024/04 | TabSQLify | [TabSQLify: Enhancing Reasoning Capabilities of LLMs Through Table Decomposition](https://arxiv.org/abs/2404.10150) | ![Static Badge](https://badgen.net/badge/color/NAACL/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/Sungwon-Han/FeatLLM) |
| 2024/04 | LLMClean | [LLMClean: Context-Aware Tabular Data Cleaning via LLM-Generated OFDs](https://arxiv.org/abs/2404.18681) | ![Static Badge](https://badgen.net/badge/color/ICLR/blue?label=) | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/asdfthefourth/LLMClean) |
| 2024/05 | CARTE | [CARTE: Pretraining and Transfer for Tabular Learning](https://openreview.net/forum?id=9kArQnKLDp) | | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/soda-inria/carte) |
| 2024/07 | folktexts | [Evaluating language models as risk scores](https://arxiv.org/abs/2407.14614) | | [![Static Badge](https://badgen.net/badge/color/Code/black?label=)](https://github.com/socialfoundations/folktexts) |
| 2024/07 | SpreadsheetLLM | [SpreadsheetLLM: Encoding Spreadsheets for Large Language Models](https://arxiv.org/abs/2407.09025) | | |



## Workshops
- [Table Representation Learning Workshop @ NeurIPS 2023](https://neurips.cc/virtual/2023/workshop/66546)
- [Table Representation Learning Workshop @ NeurIPS 2024](https://table-representation-learning.github.io/)

## Useful Blogs
- [A Short Chronology Of Deep Learning For Tabular Data](https://sebastianraschka.com/blog/2022/deep-learning-for-tabular-data.html) by [Sebastian Raschka](https://www.linkedin.com/in/sebastianraschka/)

## Citation
```
@misc{wu2024awesomellmtabular,
  author = {Hong-Wei, Wu},
  title = {Awesome-LLM-Tabular},
  year = {2024},
  note = {Accessed: 2024-05-30},
  url = {https://github.com/johnnyhwu/Awesome-LLM-Tabular},
  orcid = {https://orcid.org/0009-0005-8073-5297}
}
```

## Contributing
We welcome contributions to keep this repository up-to-date with the latest research and applications of LLM in the **tabular** domain. Whether you want to correct any mistakes, add new content, or suggest improvements, your contributions are highly appreciated :hugs:.
