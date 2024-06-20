# Evaluators in Langchain

In the `langchain` folder, you will find three types of evaluators to choose from:

### 1. String Evaluators

String Evaluators assess the predicted output for a given input by comparing it to a reference string. The following evaluation methods are demonstrated:

#### 1.1 Criteria Evaluation

- **Description**: Scores the output based on predefined criteria. For instance, if the answer matches the desired response, it scores 1; otherwise, it scores 0. You can define your criteria or use those provided by Langchain.

#### 1.2 Custom String Evaluator

- **Description**: Allows for creating custom evaluation metrics. For example, you can integrate with `huggingface/evaluate` to use metrics like perplexity.

#### 1.3 Embedding Distance

- **Description**: Measures the similarity of text based on vector embeddings.

#### 1.4 Exact Match

- **Description**: Evaluates the similarity of text by exact string matching.

#### 1.5 JSON Evaluators

- **Description**: Useful for checking if the model's output is in JSON format.

#### 1.6 Regex Match

- **Description**: Uses regular expressions to verify if the output matches specific patterns.

#### 1.7 Scoring Evaluator

- **Description**: Uses a language model to score the output based on a defined scale, such as rating responses from 1 to 10 based on how well they answer a question.

#### 1.8 String Distance

- **Description**: Measures string similarity or difference, similar to Levenshtein distance.

### 2. Comparison Evaluators

Comparison Evaluators are used to assess outputs from two different chains or models. This is useful for A/B testing, comparing outputs from different LLMs, or evaluating prompts. The following methods are demonstrated:

#### 2.1 Pairwise String Comparison

- **Description**: Compares outputs from two sources at the string level. For example, a language model might evaluate which response it prefers based on specified criteria.

#### 2.2 Pairwise Embedding Distance

- **Description**: Compares outputs from two sources at the vector level.

#### 2.3 Custom Pairwise Evaluator

- **Description**: Allows for custom comparisons between outputs from two sources.

### 3. Trajectory Evaluators

Trajectory Evaluators are designed for evaluating agents by analyzing the sequence of actions taken during a task. This is useful for evaluating the agent’s behavior and decision-making process over time.
