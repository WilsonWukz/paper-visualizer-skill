# Paper Visualizer (MCP Skill)

> **Turn ArXiv Papers into High-Fidelity Technical Schematics.**
> A specialized MCP (Model Context Protocol) skill that architects professional diagrams for research papers, optimized for Nano Banana Pro.

---

<div align="center">
  <img src="skills/visual-architect/example/Anthropic_Console.jpg" alt="Transformer Architecture - Anthropic Console" width="100%">
  <p><em>Figure 1: The "Golden Schema" generated via Anthropic Console (Claude 3.5 Sonnet). Note the precise recursive structure of the Encoder/Decoder stacks and the detailed "Multi-Head Attention" insets.</em></p>
</div>

---

## Introduction

**"Why can't AI draw my architecture correctly?"**

Researchers and Engineers often struggle to visualize complex systems. While standard generative AI excels at art, it fundamentally fails at **Scientific Logic** and **Topological Consistency**, often producing "hallucinated" connections or gibberish text.

**Paper Visualizer** bridges this gap. It acts as a **Structural Architect** middleware that:
1.  **Decodes the PDF**: Reads the raw academic text to extract the logical topology (e.g., *Is it a cyclic loop? A parallel stream? A hierarchical tree?*).
2.  **Visual Tokenization**: Translates abstract concepts (e.g., "Residual Connection") into concrete visual tokens (e.g., "Curved bypass arrow with (+) symbol").
3.  **Strict Layout Enforcement**: Outputs a structured, coordinate-based prompt that forces Nano Banana Pro to obey physical laws.

## Key Features

* **6 Cognitive Layout Engines**: Automatically selects the best visual topology for your paper:
    * `Linear Pipeline` (for CNNs/Preprocessing)
    * `Parallel Dual-Stream` (for Transformers/Siamese Networks)
    * `Central Hub` (for Agents/RL)
    * `Cyclic Loop` (for Optimization/GANs)
    * `Hierarchical Stack` (for FPNs/UNets)
    * `Matrix Grid` (for Ablation Studies)
* **Typography Guardrails**: Enforces sans-serif hierarchy rules to minimize text artifacts, ensuring that main labels (e.g., "ENCODER") remain legible.
* **Nano Banana Pro Optimized**: Specifically tuned to leverage Nano Banana Pro's strengths in text rendering and structural adherence.

## Gallery: Style Variants

This skill supports different aesthetic outputs based on the configuration passed to Nano Banana Pro.

### Variant A: "The Textbook Standard" (Precision Focus)
*(See Figure 1 above)*
* **Pipeline**: Claude 3.5 Sonnet → Nano Banana Pro
* **Style**: Clean, Academic, White Background. Perfect for **Paper Submissions (LaTeX)**.

### Variant B: "The Tech Presentation" (Impact Focus)
<div align="center">
  <img src="skills/visual-architect/example/GPT_4o_web.jpeg" alt="Transformer Architecture - GPT-4o Style" width="100%">
  <p><em>Figure 2: The same Transformer architecture rendered with a "Sci-Fi/High-Tech" aesthetic via GPT-4o logic. Ideal for <strong>Conference Slides, Posters, and Pitch Decks</strong>.</em></p>
</div>

## Benchmark & Validation

We strictly evaluate this skill across different environments to ensure robustness.

| Environment | Logic Model | Logic Adherence | Detail Insets | Log Output |
| :--- | :--- | :--- | :--- | :--- |
| **Anthropic Console** | Claude 3.5 Sonnet | Excellent | Perfect | [View Log](skills/visual-architect/example/response%20(Anthropic_Console).txt) |
| **ChatGPT Web** | GPT-4o | Very Good | Good | [View Log](skills/visual-architect/example/response%20(GPT_4o_web).txt) |

> **Observation**: Claude 3.5 Sonnet tends to follow the "Detail Inset" (Zone 7 & 8) instructions more strictly, making it the recommended engine for complex architectures.

## Installation & Usage

### Option 1: Manual Integration (Claude Desktop / Cursor)
1.  Download the core skill file: [`skills/visual-architect/SKILL.md`](skills/visual-architect/SKILL.md).
2.  Add it to your **Project Knowledge** or **System Instructions**.
3.  **Trigger**: "Generate a visual schema for this paper's methodology."

### Option 2: MCP Integration
This repository is structured as an MCP collection. You can point your MCP client to the `skills/visual-architect` directory to load this specific capability.

## How It Works (The Prompt Engineering)

This skill forces the LLM to output a structured JSON-like Markdown block, bypassing its usual "chatty" nature:

```markdown
[LAYOUT CONFIGURATION]
* Selected Layout: Parallel Dual-Stream
* Composition Logic: Left column = Encoder... Right column = Decoder...

[ZONE 1: INPUT]
* Visual Structure: A stack of 3 realistic paper icons...
...