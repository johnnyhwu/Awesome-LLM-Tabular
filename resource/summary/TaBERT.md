# Summarization

## Approach

1. Content Snapshot Creation:
- The paper discusses creating snapshots based on the relevance between an utterance and a row.
- For multiple rows, the top-K rows in the input table with the highest n-gram overlap ratio with the utterance are selected.
- For a single row, a synthetic row is created by selecting cell values from each column that have the highest n-gram overlap with the utterance. This approach is motivated by the idea that relevant cell values could come from multiple rows. For instance, if the utterance is about comparing participants in 2008 to the London Olympics, and the table has columns like Year, Host City, and Number of Participants, the relevant cells could come from different rows. Synthetic rows help in capturing this information and also stabilize learning.

2. Row Linearization with TABERT
- TABERT is introduced, which creates a linearized sequence for each row in the content snapshot as input to a Transformer model.
- This linearization consists of a concatenation of the utterance, columns, and their cell values. Each cell is represented by the name and data type of the column, along with its actual value, separated by a vertical bar.

## Experiment

WIKITABLEQUESTIONS Results:
- The paper presents results on the WIKITABLEQUESTIONS dataset.
- The MAPO system augmented with a TABERTLarge model with three-row content snapshots, labeled as TABERTLarge(K = 3), achieved a single-model exact-match accuracy of 52.3% on the test set. This surpasses the previously best ensemble system (46.9%) from Agarwal et al. (2019) by an absolute 5.4%.

Table 1: Execution accuracies on WIKITABLEQUESTIONS:
- Base Parser (from Liang et al. 2018) achieved a DEV best of 42.7% and a TEST best of 43.8%.
- Using BERTBase (K = 1), the DEV best was 50.4% and the TEST best was 49.2%.
- With TABERTBase (K = 1), the results were 51.6% for DEV best and 51.2% for TEST best.
- TABERTBase with K = 3 achieved a DEV best of 52.4% and a TEST best of 51.3%.
- Using BERTLarge (K = 1), the DEV best was 50.8% and the TEST best was 50.1%.
- TABERTLarge (K = 1) achieved a DEV best of 52.7% and a TEST best of 51.5%.
- Finally, TABERTLarge with K = 3 achieved the highest DEV best of 53.0% and a TEST best of 52.3%.