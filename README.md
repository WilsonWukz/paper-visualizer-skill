# Paper Visualizer (MCP Skill)

> **Turn ArXiv Papers into High-Fidelity Technical Schematics.**
> A specialized MCP (Model Context Protocol) skill that architects professional diagrams for research papers, optimized for Nano Banana.

![Hero Demo](skills/visual-architect/example/demo%20(Attention%20Is%20All%20You%20Need-method).jpeg)
*Figure 1: Transformer Architecture generated purely from the original paper's text using this skill.*

## Why use this?

Researchers and Engineers spend hours drawing diagrams in PowerPoint/Visio. Generative AI (DALL-E/Midjourney) usually fails at scientific logic, creating "hallucinated" structures.

**Paper Visualizer** solves this by acting as a **"Structural Architect"**:
1.  **Analyzes Logic**: Reads the paper (PDF/Text) and identifies the topology (e.g., Linear Pipeline, Cyclic Loop, Parallel Stream).
2.  **Enforces Physics**: Translates abstract concepts into concrete physical objects (Stacks, Gears, Flows).
3.  **Strict Formatting**: Outputs a "Golden Schema" prompt that strictly controls layout and typography.

## Features

- **6 Pre-defined Layout Engines**: Automatically detects if your paper needs a *Linear Pipeline*, *Central Hub*, *Matrix Grid*, etc.
- **Text-Rendering Optimization**: Enforces sans-serif typography and hierarchy rules to minimize AI spelling errors.
- **Zone-Based Composition**: Breaks complex systems into 2-5 distinct physical zones for precise control.

## Installation & Usage

### Option 1: Use with Claude Desktop / Cursor (Manual)
1.  Locate the core skill file: `skills/visual-architect/SKILL.md`.
2.  Add it to your Project Knowledge or System Instructions.
3.  **Trigger**: "Generate a visual schema for this paper's methodology."

### Option 2: MCP Server Integration
This repository is structured as an MCP collection. You can point your MCP client to the `skills/visual-architect` directory to load this specific capability.

## Gallery: Before & After

### Case Study: "Attention Is All You Need" (Transformer)

**Step 1: Input**
> "I am uploading the methodology section of the 'Attention Is All You Need' paper. Generate the schema."
> *(See original input: [skills/visual-architect/example/test prompt.txt](skills/visual-architect/example/test%20prompt.txt))*

**Step 2: AI Architect Output (The Intermediate Prompt)**
The skill automatically selected the **Parallel Dual-Stream Layout** (Encoder vs Decoder).
*View the full generated prompt log:* [skills/visual-architect/example/response (GPT-4o).txt](skills/visual-architect/example/response%20(GPT-4o).txt)

**Step 3: Final Render (Midjourney v6)**
![Architecture Variant](skills/visual-architect/example/demo%20(Attention%20Is%20All%20You%20Need-method).jpeg)
*Note the precise separation of the Encoder Stack (Left) and Decoder Stack (Right), connected by the Cross-Attention mechanism.*

## Prompting Guide (How it works)

This skill forces the LLM to output a structured JSON-like Markdown block:

```markdown
[LAYOUT CONFIGURATION]
* Selected Layout: Parallel Dual-Stream
* Composition Logic: Left column = Encoder... Right column = Decoder...

[ZONE 1: INPUT]
* Visual Structure: A stack of 3 realistic paper icons...