# Summarization

## Approach

- **LIFT Training**
  - To fine-tune a pretrained LM with LIFT on a target task, two steps are applied:
    - Convert each sample into a sentence using a fixed template.
    - Fine-tune LMs with these sentence datasets using the default cross-entropy loss for token prediction.
  - A generic template is used to convert samples into sentences. For instance, if a sample has p attributes, the template might be: "When we have x1=r.x1, x2=r.x2, ..., xp=r.xp, what should be y?". The actual prompts are provided in a later section of the paper.
- **LIFT Inference:**
  - For inference, the same prompt template is used, excluding the answer and end-of-answer parts.
  - Once the fine-tuned LM completes the test prompt, the output tokens are parsed.
  - For classification tasks, the generated text is compared with the string representation of the class names.
  - For regression tasks, the generated string is converted into a number. For example, if the output is “y=10.35@@@extratokens”, the value “10.35” is parsed as the final prediction.

The paper also mentions potential issues with the generated output. For classification, the output string might not match any actual class, which is considered a misclassification. For regression, the output might be invalid if the string-to-number parsing fails. In such cases, the generation randomness is adjusted by modifying the decoding temperature.

## Experiment

1. **Decision Boundaries:**
- LIFT/GPT models adapt well to different decision boundaries and capture their rough shapes. The boundary shapes are axis-parallel, similar to tree-based classifiers. They also show fractals similar to some convolution neural networks.

2. **Robustness:**
- The paper investigates the robustness of LIFT against outlier samples in training data and feature corruption on test data.
- For regression tasks with outliers, LIFT is robust to outliers in the training data.

3. **Summary of Main Findings:**
- On various classification tasks, LIFT achieves accuracies comparable to strong baselines.
- For regression, LIFT approximates different types of low-dimensional functions but struggles with high-dimensional cases.
- LIFT is robust to outliers in training data for regression tasks.
- LIFT can be improved on classification tasks by designing prompts to specify feature names and the target task.
- Warming up LIFT with pretext tasks using synthetic data improves prediction performance, especially in the low-data regime.
- For classification tasks, training with augmented data significantly improves LIFT's tolerance against perturbed test data.