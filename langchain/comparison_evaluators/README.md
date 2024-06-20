# Comparison Evaluators

Comparison Evaluators in LangChain are designed to compare the outputs of two different chains or language models (LLMs). They are particularly useful for tasks such as A/B testing between two models, comparing different versions of the same model, or generating preference scores for AI-assisted reinforcement learning.

### Overview

Comparison Evaluators inherit from the `PairwiseStringEvaluator` class, which provides an interface for comparing two strings. Typically, these strings represent outputs from different prompts, models, or versions of the same model. The evaluator assesses the pair of strings and returns a dictionary containing an evaluation score and other relevant details.

### Custom Comparison Evaluator

To create a custom comparison evaluator, follow these steps:
1. Inherit from the `PairwiseStringEvaluator` class.
2. Overwrite the `evaluate_string_pairs` method for synchronous evaluations.
3. If asynchronous evaluation is needed, overwrite the `aevaluate_string_pairs` method.

### Key Methods

- **`evaluate_string_pairs`**: This method evaluates pairs of output strings. It should be overwritten when creating custom evaluators.
- **`aevaluate_string_pairs`**: This method asynchronously evaluates pairs of output strings. It should be overwritten for asynchronous evaluation.

### Key Properties

- **`requires_input`**: Indicates whether the evaluator requires an input string.
- **`requires_reference`**: Specifies whether the evaluator needs a reference label.