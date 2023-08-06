# Summarization

## ChatGPT

### Approach
This paper presents TabLLM, a few-shot classification technique for tabular data using large language models. The approach involves prompting a large language model with a serialization of the tabular data to a natural-language string, together with a short description of the classification problem. In the few-shot setting, the large language model is fine-tuned using some labeled examples. The paper evaluates several serialization methods including templates, table-to-text models, and large language models. Despite its simplicity, the technique outperforms prior deep-learning-based tabular classification methods on several benchmark datasets. In most cases, even zero-shot classification obtains non-trivial performance, illustrating the method’s ability to exploit prior knowledge encoded in large language models. Unlike many deep learning methods for tabular datasets, this approach is also competitive with strong traditional baselines like gradient-boosted trees, especially in the very-few-shot setting.

### Experiment
The paper experiments with nine different serializations and the T0 language model of different sizes to evaluate the performance of TabLLM for zero- and few-shot tabular classification. The authors use the parameter-efficient fine-tuning method T-Few to update the LLM’s parameters using some labeled examples. They also evaluate GPT-3 in the zero-shot setting. The authors find that the TabLLM technique outperforms prior deep-learning-based tabular classification methods on several benchmark datasets. In most cases, even zero-shot classification obtains non-trivial performance, illustrating the method’s ability to exploit prior knowledge encoded in large language models. The authors also perform additional experiments for alternative concept names and found no consistent performance difference even though there were considerable differences in the concept names. Finally, the authors provide runtime estimates for TabLLM on the Income dataset for 64 training examples and 30 epochs with a batch size of 8, which was less than 3 minutes.

## Human

TBA