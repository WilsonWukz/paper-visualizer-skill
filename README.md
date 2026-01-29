# Paper Visualizer (MCP Skill)

> **Turn ArXiv Papers into High-Fidelity Technical Schematics.**
> A specialized MCP (Model Context Protocol) skill that architects professional diagrams for research papers, optimized for Midjourney v6 & DALL-E 3.

![Hero Demo](skills/visual-architect/example/Anthropic_Console.jpg)
*Figure 1: Transformer Architecture generated via Anthropic Console (Claude 3.5 Sonnet) using this skill. Note the precise "Multi-Head Attention" detail insets.*

## Why use this?

Researchers and Engineers spend hours drawing diagrams in PowerPoint/Visio. Generative AI usually fails at scientific logic, creating "hallucinated" structures.

**Paper Visualizer** solves this by acting as a **"Structural Architect"**:
1.  **Analyzes Logic**: Reads the paper (PDF/Text) and identifies the topology (e.g., Linear Pipeline, Cyclic Loop, Parallel Stream).
2.  **Enforces Physics**: Translates abstract concepts into concrete physical objects (Stacks, Gears, Flows).
3.  **Strict Formatting**: Outputs a "Golden Schema" prompt that strictly controls layout and typography.

## Features

- **6 Pre-defined Layout Engines**: Automatically detects if your paper needs a *Linear Pipeline*, *Central Hub*, *Matrix Grid*, etc.
- **Text-Rendering Optimization**: Enforces sans-serif typography and hierarchy rules to minimize AI spelling errors.
- **Zone-Based Composition**: Breaks complex systems into 2-5 distinct physical zones for precise control.

## Installation & Usage

### Option 1: Manual Integration (Claude Desktop / Cursor)
1.  Locate the core skill file: [`skills/visual-architect/SKILL.md`](skills/visual-architect/SKILL.md).
2.  Add it to your Project Knowledge or System Instructions.
3.  **Trigger**: "Generate a visual schema for this paper's methodology."

### Option 2: MCP Integration
This repository is structured as an MCP collection. You can point your MCP client to the `skills/visual-architect` directory.

## Benchmark & Validation

We strictly evaluate this skill across different environments to ensure robustness.

### Case Study: "Attention Is All You Need" (Transformer)

**Input Context:**
> User uploaded the methodology section of the Transformer paper.
> *(See input: [skills/visual-architect/example/test prompt.txt](skills/visual-architect/example/test%20prompt.txt))*

**Benchmark Results:**

| Environment | Model | Log Output | Result Image |
| :--- | :--- | :--- | :--- |
| **Anthropic Console** | Claude 3.5 Sonnet | [View Log](skills/visual-architect/example/response%20(Anthropic_Console).txt) | **[See Hero Image]** |
| **ChatGPT Web** | GPT-4o | [View Log](skills/visual-architect/example/response%20(GPT_4o_web).txt) | [View Result](skills/visual-architect/example/GPT_4o_web.jpeg) |

*The Anthropic Console run demonstrated superior adherence to the "Detail Inset" instructions (Zone 7 & 8).*

## Prompting Guide (How it works)

This skill forces the LLM to output a structured JSON-like Markdown block:

```markdown
[LAYOUT CONFIGURATION]
* Selected Layout: Parallel Dual-Stream
* Composition Logic: Left column = Encoder... Right column = Decoder...

[ZONE 1: INPUT]
* Visual Structure: A stack of 3 realistic paper icons...
...

```

## License

MIT License. Copyright (c) 2026 WilsonWukz.