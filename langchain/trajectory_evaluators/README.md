# Trajectory Evaluators

Trajectory Evaluators in LangChain offer a comprehensive approach to evaluating an agent's performance. By assessing the entire sequence of actions and responses—referred to as the "trajectory"—these evaluators provide a more thorough measurement of an agent's effectiveness and capabilities.

### Overview

A Trajectory Evaluator implements the `AgentTrajectoryEvaluator` interface, which includes two essential methods:

- **`evaluate_agent_trajectory`**: Synchronously evaluates an agent's trajectory.
- **`aevaluate_agent_trajectory`**: Asynchronously evaluates the trajectory, allowing for parallel execution to enhance efficiency.

### Parameters

Both methods require the following parameters:

- **`input`**: The initial input provided to the agent.
- **`prediction`**: The agent's final predicted response.
- **`agent_trajectory`**: The sequence of intermediate steps taken by the agent, represented as a list of tuples.

### Return Values

The methods return a dictionary, typically containing:
- **`score`**: A float representing the agent's effectiveness.
- **`reasoning`**: A string explaining the rationale behind the score.

### Capturing Trajectory

To capture an agent's trajectory, initialize the agent with the parameter `return_intermediate_steps=True`. This enables the collection of all intermediate steps without the need for special callbacks.


