# Evaluate_llm

This repository demonstrates evaluation methods for LLM (Large Language Model) applications. The objective is to showcase how to evaluate LLM applications using three frameworks: Langchain, DeepEval, and Langsmith.

## Purpose

The purpose of this repository is to provide a demonstration of evaluating LLM applications using the following three frameworks:
- **Langchain**
- **DeepEval**
- **Langsmith**

## Evaluation Frameworks

### 1. Langchain

Langchain is a framework designed for developing applications that integrate LLMs. It includes components for evaluating model responses, such as string evaluation and comparison evaluation.

#### Key Features
- **Ease of Use:** Simple to implement for basic evaluations.
- **Basic Metrics:** Supports exact match evaluation and JSON output checking.

#### Limitations
- **Custom Prompts Required:** AI scoring metrics require custom prompt creation.
- **Limited Traceability:** Does not support result tracing.

### 2. DeepEval

DeepEval is an open-source framework focused on evaluating language models. It includes over 14 evaluation metrics and can synthesize test datasets. Additionally, it supports unit testing.

#### Key Features
- **Comprehensive Metrics:** Supports a wide range of current LLM evaluation metrics.
- **Decision-Making:** Suitable for evaluations requiring LLM-driven decisions.

#### Limitations
- **Complexity:** Slightly more complex code compared to Langchain.

### 3. Langsmith

Langsmith extends Langchain for enhanced monitoring and tracking of Q&A performance. It integrates seamlessly with Langchain for improved result monitoring.

#### Key Features
- **Action Monitoring:** Tracks LLM actions and supports version history.
- **No-Code Evaluations:** Enables no-code evaluations (not covered in this example).

#### Limitations
- **Custom Metrics:** Most metrics require custom creation or integration through Langchain.

## Recommendations

For a quick overview, explore the `langsmith` folder. It demonstrates the integration of Langsmith with Langchain and DeepEval for metric evaluation. This integration provides valuable insights and a potential development path for future products.
