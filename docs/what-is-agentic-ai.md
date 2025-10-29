# What is Agentic AI?

## Introduction

Many of us currently use Large Language Models (LLMs) by prompting them to complete tasks in a single pass. For example, we might ask an LLM to "write an essay on topic X." This approach is similar to asking a human to write an essay from the first word to the last word in one continuous flow, without ever using backspace.

However, humans don't produce their best work under such constraints—writing linearly without revision or iteration. Neither do AI models. Despite these limitations, LLMs perform surprisingly well with this approach.

## Agentic Workflows: A Better Approach

In contrast, an **agentic workflow** breaks down complex tasks into multiple iterative steps:

1. **Planning**: Create an outline or plan
2. **Research**: Identify what information is needed and conduct web research
3. **Drafting**: Write an initial version based on gathered information
4. **Review**: Analyze the draft to identify areas needing revision or additional research
5. **Revision**: Refine and improve the work iteratively
6. **Human-in-the-loop** (optional): Request human review for critical facts or decisions

This iterative process mirrors how humans naturally work: thinking, researching, revising, and iterating. While agentic workflows may take longer than single-prompt approaches, they consistently deliver superior results.

## Definition of Agentic AI Workflows

An **agentic AI workflow** is a process where an LLM-based application executes multiple sequential steps to complete a task. Each step may involve:

- Using an LLM to generate content or make decisions
- Calling external APIs (e.g., web search, data retrieval)
- Processing and synthesizing information
- Iterating based on feedback or reflection

### Example: Essay Writing Workflow

1. **Outline Generation**: Use an LLM to create an essay outline
2. **Research Planning**: Use an LLM to determine search terms for web research
3. **Information Gathering**: Call web search APIs to retrieve relevant pages
4. **Draft Creation**: Feed downloaded content into an LLM to write the first draft
5. **Reflection**: Use an LLM to analyze the draft and identify improvement areas
6. **Human Review** (optional): Request human feedback on key facts or assertions
7. **Revision**: Based on feedback, revise and refine the draft

This multi-step process produces significantly better output than a single linear prompt.

## Key Skills for Building Agentic Workflows

Building effective agentic workflows requires mastering two critical skills:

### 1. Task Decomposition

The ability to break complex tasks into smaller, manageable steps that can be executed sequentially. This involves:

- Identifying natural breakpoints in a task
- Understanding dependencies between steps
- Designing workflow logic that guides the agent through the process

### 2. Component Design

Creating robust components that execute individual steps effectively. Each component must:

- Handle specific subtasks reliably
- Integrate seamlessly with other workflow components
- Manage errors and edge cases gracefully

Mastering these skills is essential for building agentic workflows across a wide range of applications.

## Example: Research Agent

A practical example of an agentic workflow is a **research agent**. This agent takes a research topic as input and produces a comprehensive research report through multiple steps.

### Workflow Process

1. **Planning**: Determine what research needs to be conducted
2. **Web Search**: Call web search engines to find relevant sources
3. **Information Retrieval**: Download and process web pages
4. **Synthesis**: Synthesize and rank findings from multiple sources
5. **Outline Creation**: Draft a structured outline for the report
6. **Editor Review**: Use an editor agent to review for coherence and quality
7. **Report Generation**: Generate a comprehensive markdown report

### Example Output

For a research topic like "How do I build a new rocket company to compete with SpaceX?", the research agent would:

- Find and download multiple relevant sources
- Analyze the information deeply
- Structure findings into sections (Introduction, Background, Findings, etc.)
- Provide thoughtful insights and appropriate caveats

The resulting report is significantly more thoughtful and comprehensive than what a single prompt would produce.

### Applications

Research agents have practical applications across various domains:

- **Legal**: Document analysis and compliance research
- **Healthcare**: Medical research and literature review
- **Business**: Product research and competitive analysis
- **Academic**: Literature review and research synthesis

## Autonomy in Agentic Workflows

Agentic workflows can vary significantly in their level of autonomy:

- **Highly Autonomous**: Complex workflows that execute many steps with minimal human intervention
- **Moderately Autonomous**: Workflows that include strategic human checkpoints
- **Low Autonomy**: Simpler workflows with frequent human oversight

The degree of autonomy depends on the specific use case, complexity of the task, and the level of confidence required in the output. Simpler workflows can still provide significant value even with lower autonomy.

## Conclusion

Agentic AI workflows represent a fundamental shift from single-prompt interactions to multi-step, iterative processes. By breaking down complex tasks into manageable steps and executing them systematically, agentic workflows enable LLMs to produce higher-quality outputs across a wide range of applications.

The key to building effective agentic workflows lies in understanding how to decompose tasks and design robust components that work together seamlessly. These skills unlock the potential to create powerful AI applications that can tackle complex, real-world problems.

