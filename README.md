# KNOWY: Agentic Knowledge System

**Agentic Multimodal Architecture for Personal Knowledge Compilation, Epistemic Evolution, and Expert-Level Reasoning**

## Overview
KNOWY represents a paradigm shift from retrieval-oriented personal AI tools toward epistemic infrastructures. Instead of treating personal knowledge as a static repository, KNOWY builds an evolving epistemic foundation that guarantees integrity, correctness, and deep understanding.

The system addresses the fundamental challenge of epistemic integrity in personal AI systems through a rigorously layered architecture that distinguishes between shallow operational agents and deep epistemic agents.

## Core Design Principles
- **Epistemic Integrity Over Access**: Prioritizes correctness, uncertainty quantification, and hallucination prevention over comprehensive retrieval.
- **Local-First Operation**: Ensures privacy, reproducibility, and system composability through command-line interfaces and local model execution.
- **Multimodal Native**: Treats video, diagrams, and text as first-class knowledge modalities with specialized processing pipelines.
- **Shallow-Deep Agent Separation**: Enforces strict boundaries between operational agents (bounded transformations) and epistemic agents (boundary-crossing reasoning).

## System Architecture
KNOWY implements an 8-layer architecture orchestrated via **LangGraph**:

1.  **Layer 0: Universal Ingestion** - Normalizes heterogeneous inputs (browser, API, manual) into canonical descriptors.
2.  **Layer 1: Exploration & Expansion** - Performs deep link analysis and reference expansion to find hidden artifacts.
3.  **Layer 2: Multimodal Acquisition** - Specialized pipelines for text, video (shot segmentation), and code.
4.  **Layer 3: Multi-Resolution Representation** - Maintains explicit abstraction hierarchies from raw data to synthesis.
5.  **Layer 4: Classification & Ontology** - Dynamic categorization and relationship mapping.
6.  **Layer 5: Expert Reasoning & Teaching** - Pedagogical synthesis and gap analysis.
7.  **Layer 6: Diagrammatic Explanation** - Automated schematic generation for enhanced understanding.
8.  **Layer 7: Deep External Research (DERA)** - Controlled external inquiry for knowledge evolution.

## Key Innovations
- **Video-as-Knowledge Pipeline**: Integration of `video-analyzer` for shot segmentation, transcript alignment, and visual-semantic extraction.
- **Diagrammatic Explanation**: Automated generation of pedagogical diagrams using Graphviz/Mermaid.
- **CLI-First Interaction**: Built on the `llm` framework for scriptability and workflow integration.
- **Versioned Knowledge Evolution**: Temporal knowledge management with explicit uncertainty tracking.

## Technology Stack

| Component | Technology | Description |
|-----------|------------|-------------|
| **Orchestration** | LangGraph | Graph-based execution with conditional routing |
| **Local Runtime** | Ollama | Unified API for local models (Llama 3.x, Qwen, Gemma) |
| **Vision Model** | LLaMA 3.2 Vision | Native image understanding for video frames |
| **Video Analysis** | video-analyzer | Shot segmentation and transcript alignment |
| **CLI Framework** | llm | Plugin architecture and model abstraction |
| **Vector DB** | FAISS / Qdrant | High-performance similarity search |
| **Storage** | PostgreSQL + Neo4j | Relational metadata + graph ontologies |
| **Diagrams** | Graphviz, Mermaid | Programmatic schematic creation |

## Documentation
Full technical design details and architectural diagrams can be found in the [`doc/`](./doc) directory.
