# Deepeval

The `deepeval` folder contains various components and processes for utilizing the Deepeval framework. Below is an overview of the purpose of each subfolder within `deepeval`:

## 1. Test Cases

- **Purpose**: Serves as a template for storing all relevant variables used in evaluating and testing language models.
- **Contents**: Each test case includes `input`, `actual_output`, `expected_output`, `context`, and `retrieval_context`. Different metrics might require varying combinations of these variables.
- **Function**: Facilitates the evaluation of language models by comparing model outputs against expected outcomes.

## 2. Dataset

- **Purpose**: Aggregates multiple test cases.
- **Function**: Represents a collection of Q&A pairs bundled together for evaluation. A single test case corresponds to one Q&A pair, while a dataset consists of multiple test cases for comprehensive assessment.

## 3. Synthesizer

- **Purpose**: Generates evaluation datasets by synthesizing input data and responses using a language model.
- **Function**: Automates the creation of test data and answers, which can be based on provided documents or existing context.

## 4. Metric

- **Purpose**: Measures the performance of language models in answering questions.
- **Contents**: Includes various metrics used to evaluate model capabilities, ensuring comprehensive performance assessment.

## 5. Benchmarks

- **Purpose**: Provides standard LLM evaluation methods using benchmark datasets.
- **Function**: Compares model scores against global benchmarks, enabling performance comparisons with other language models.

### Note

Focus primarily on `Test Cases` and `Metric` folders as they are essential for integrating with Langsmith to trace individual results. The `Benchmarks` folder is less critical unless you are building or fine-tuning new models.
