# PhiAgent

## Author
**Phi Nguyen Xuan - AI Intern**

## Overview
PhiAgent is an advanced agent designed to facilitate intelligent interactions with users by leveraging various tools and a powerful language model. It is built to handle complex queries, perform web searches, and provide detailed responses based on the latest information available online.

## Features

### Asynchronous Mechanism
PhiAgent utilizes an asynchronous programming model, allowing it to handle multiple tasks concurrently without blocking the execution flow. This is particularly beneficial for operations that involve waiting for external resources, such as web requests or API calls. The asynchronous design enhances the responsiveness of the agent, enabling it to process user inputs and return results efficiently.

Key aspects of the asynchronous mechanism include:
- **Non-blocking I/O**: The agent can perform web searches and fetch data without halting other operations, ensuring a smooth user experience.
- **Event-driven architecture**: The agent responds to events (like user inputs) and processes them in an efficient manner, allowing for real-time interactions.

### Stream Reasoning Steps
PhiAgent incorporates a unique stream reasoning feature that allows it to provide insights and reasoning as it processes user queries. This feature enhances transparency and helps users understand the decision-making process of the agent.

The stream reasoning steps include:
1. **Tool Selection**: The agent evaluates the input and selects appropriate tools to gather information. This is done through the `ToolSelection` mechanism, which identifies the best tools based on the query context.
2. **Execution of Tools**: Once the tools are selected, the agent executes them asynchronously, allowing for quick retrieval of data.
3. **Response Generation**: The agent compiles the results and generates a coherent response, which is then streamed back to the user. This process is facilitated by the `ResponseStreamEvent`, which allows the agent to communicate its reasoning step-by-step.

