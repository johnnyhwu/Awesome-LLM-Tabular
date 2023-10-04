# Summarization

## Approach

- **Fine-Tuning Phase**
  - The goal of this phase is to adapt current state-of-the-art NLP architectures, such as GPT, BERT, and their extensions, to the task of selecting the most relevant features from each of the linked external source entities.
  - Two common fine-tuning methods are highlighted: task-specific fine-tuning (performed on the target dataset) and preliminary fine-tuning (applied on other datasets). While task-specific fine-tuning is more prevalent, recent studies have shown that applying both (preliminary followed by task-specific) yields superior results.
  - The primary challenge in applying preliminary fine-tuning to tabular datasets is their diversity in terms of domains, number of classes, feature composition, etc. This diversity makes training a universal feature engineering tool challenging.
- **Preliminary Fine-Tuning with Dataset Task Reformulation**
  - A significant challenge in learning from multiple tabular datasets is their varying number of classes. This makes using a single output layer with a fixed number of entries unfeasible.
  - To address this, for each dataset, there's a set of free texts, each associated with an entity in the dataset. For each text, a Cartesian product is created, pairing the text with all possible target class values. This transforms the problem into one of Sentence-pairs classification.
  - In this setting, a set consisting of three elements is presented: the text (first sentence), a possible target class value (second sentence), and the label. The label is set to True if the pair belongs to the set of text and target class values.
- **Linking External Source Entities**
  - Each dataset entity has a linked Wikipedia entity. The abstracts of these entities are then extracted using DBpedia.

## Experiment

- **Evaluating the Efficacy of the Fine-Tuning Method**
  - The experiment focused on the efficacy of the features generated from the external data source, specifically DBpedia unstructured text. The classifiers were trained only on the generated features.
  - Results for various datasets were presented in Table 1, where the proposed approach "Reformulated" was compared against two leading baselines: "Target" fine-tuning and "MT-DNN". The "Reformulated" approach outperformed the baselines in many datasets, achieving the highest results in 9 out of 17 datasets. In terms of AUC, the "Reformulated" fine-tuning improved upon the baselines by varying percentages, with significant improvements noted in some datasets.
  - Using a paired t-test, it was determined that the "Reformulated" fine-tuning outperformed the three baselines with a significance level of p < 0.001.
- **Evaluating FeSTE using Additional Entity Linking Approaches**
  - The goal of this experiment was to determine if the proposed approach, FeSTE, is generic enough to be applied with different forms of entity linking. The performance of FeSTE was evaluated when the Google-based entity linking approach was replaced by the recently proposed FGSES approaches.
  - Results for this experiment were presented in Table 3, where the full proposed approach "Reformulated" was compared against versions of the approach that utilized baseline fine-tuning methods. The results obtained on the joint set of features (original and generated) were presented, and the performance achieved by the original set of dataset features was included as a reference.