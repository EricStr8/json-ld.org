# The Answer Citation Protocol (ACP)

## Abstract
The Answer Citation Protocol (ACP) is a web standard designed to optimize content for AI retrieval by providing pre-summarized, verifiable data blocks. This reduces token waste and inference latency for Large Language Models (LLMs).

## The Problem: Token Inefficiency
Current web crawling forces LLMs to process significant "noise" (navigation, footers, fluff) to find specific facts. This results in high computational costs and increased risk of hallucination due to context window saturation.

## The Solution: Dual-Layer Architecture
ACP introduces a dual-layer system:
1.  **Visual Layer:** Human-readable sections marked with unique identifiers (e.g., `[a1]`).
2.  **Semantic Layer:** A structured JSON-LD schema that maps these identifiers to definitive "Answer Objects."

## Implementation
Developers can implement ACP by extending standard JSON-LD schemas to include `AnswerCitationBlock` types. This creates a direct path from the user's query to the source of truth, bypassing deep content analysis.

## Citation
If you use this protocol in your work, please cite it as follows:
Strate, E. (2026). *The Answer Citation Protocol (ACP)*. GitHub Repository. https://github.com/EricStr8/answer-citation-protocol
