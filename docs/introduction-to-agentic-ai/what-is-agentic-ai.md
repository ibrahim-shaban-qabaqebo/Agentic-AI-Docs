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

### The Spectrum of Autonomy

Agents can be autonomous to different degrees. Rather than viewing autonomy as a binary property—where a system is either an agent or not—it's more productive to consider autonomy as a spectrum. This perspective acknowledges that systems can be **agentic** to varying degrees, allowing us to focus on building effective systems rather than debating terminology.

The term "agentic" emerged precisely to address this nuance. By using it as an adjective rather than a binary classification, we acknowledge that different systems exhibit different levels of autonomy while recognizing that all of them contribute value to the field of agentic AI.

### Less Autonomous Agents

**Less autonomous agents** follow a predetermined sequence of steps, with most decisions hard-coded by the engineer. These agents typically:

- Execute a fully deterministic sequence of steps
- Have their workflow steps predetermined in advance
- Use tools that are hard-coded by the human engineer
- Exhibit autonomy primarily in the text the LLM generates

#### Example: Essay Writing Agent with Fixed Steps

Consider an agent designed to write an essay about black holes:

1. **Fixed Search Generation**: The agent generates a few web search queries (LLM)
2. **Predetermined Web Search**: Calls a web search engine (hard-coded step)
3. **Fixed Retrieval**: Fetches web pages based on search results (hard-coded step)
4. **Essay Generation**: Uses retrieved content to write the essay (LLM)

In this less autonomous approach, the sequence is linear and deterministic—the engineer decides in advance that the agent will always search the web, fetch results, and then write the essay. This approach works well for many applications and provides predictable, reliable behavior.

### More Autonomous Agents

**More autonomous agents** grant the LLM decision-making authority over the workflow itself. These agents:

- Allow the LLM to decide the sequence of steps dynamically
- Let the LLM choose which tools to use and when
- Trust the LLM to make strategic decisions about execution
- Determine the workflow path at runtime rather than in advance

#### Example: Essay Writing Agent with Dynamic Decisions

For the same essay-writing task, a more autonomous agent might:

1. **Dynamic Decision**: The LLM decides whether to search the web, check recent news sources, or search research paper archives
2. **Tool Selection**: Based on the decision, the agent calls the chosen tool (e.g., web search engine)
3. **Flexible Retrieval**: The LLM decides how many web pages to fetch or whether to convert PDFs to text
4. **Iterative Improvement**: After writing an initial draft, the LLM decides whether to reflect and improve, fetch more information, or produce the final output

In this more autonomous approach, the exact sequence of steps is determined by the LLM during execution, not predetermined by the programmer. This provides greater flexibility but requires more careful design to ensure reliability.

### Highly Autonomous Agents

At the far end of the spectrum, **highly autonomous agents** make extensive decisions autonomously, including:

- Deciding the complete sequence of steps needed to accomplish a task
- Choosing which tools to use and in what order
- Creating new functions or tools when needed
- Adapting their strategy based on intermediate results

These agents represent an active area of research, as they offer the most flexibility but also present challenges in terms of controllability and predictability.

### Semi-Autonomous Agents

**Semi-autonomous agents** occupy the middle ground, where:

- The agent can make some decisions autonomously
- Tool selection is flexible, but tools are usually predefined
- The workflow has some structure but allows for dynamic choices
- Balance between control and flexibility

### Choosing the Right Level of Autonomy

The appropriate level of autonomy depends on your specific application:

- **Less Autonomous**: Ideal when you need predictable, reliable behavior and can determine the optimal workflow in advance. Many valuable business applications exist at this end of the spectrum.
- **More Highly Autonomous**: Suited for complex, exploratory tasks where the optimal path isn't known in advance. These systems are less easily controllable and more unpredictable, requiring active research and careful design.

Throughout this documentation, you'll learn how to build applications at any point along this spectrum. Each approach has its place, and understanding when to use each level of autonomy is a key skill in building effective agentic systems.

## Next Steps

Now that you understand what agentic AI is and the different levels of autonomy, learn about the **[Benefits of Agentic Workflows](benefits-of-agentic-workflows.md)** to understand why these approaches are so powerful and valuable.

## Conclusion

Agentic AI workflows represent a fundamental shift from single-prompt interactions to multi-step, iterative processes. By breaking down complex tasks into manageable steps and executing them systematically, agentic workflows enable LLMs to produce higher-quality outputs across a wide range of applications.

The key to building effective agentic workflows lies in understanding how to decompose tasks and design robust components that work together seamlessly. These skills unlock the potential to create powerful AI applications that can tackle complex, real-world problems.

