# String Evaluators

String Evaluators in LangChain are components designed to assess the performance of language models by comparing their generated outputs (predictions) against a reference string or input. This comparison is essential for evaluating the accuracy or quality of the generated text, providing insights into the model's performance.

### Overview

String Evaluators typically compare a predicted string with a given input, such as a question or prompt. They may also use a reference label or context string to define what a correct or ideal response should be. These evaluators can be customized to meet the specific requirements of your application.

### Custom String Evaluator

To create a custom string evaluator, you should:
1. Inherit from the `StringEvaluator` class.
2. Implement the `_evaluate_strings` method for synchronous evaluations.
3. If asynchronous support is needed, implement the `_aevaluate_strings` method.

### Key Attributes

- **`evaluation_name`**: Specifies the name of the evaluation.
- **`requires_input`**: A boolean that indicates whether the evaluator needs an input string. 
  - If `True`, the evaluator will raise an error if the input is not provided.
  - If `False`, a warning will be logged if an input is provided, indicating it will be ignored in the evaluation.
- **`requires_reference`**: A boolean that specifies whether the evaluator needs a reference label.
  - If `True`, the evaluator will raise an error if the reference is not provided.
  - If `False`, a warning will be logged if a reference is provided, indicating it will be ignored in the evaluation.

### Key Methods

- **`aevaluate_strings`**: Asynchronously evaluates the output of the Chain or Language Model, supporting optional input and label.
- **`evaluate_strings`**: Synchronously evaluates the output of the Chain or Language Model, supporting optional input and label.