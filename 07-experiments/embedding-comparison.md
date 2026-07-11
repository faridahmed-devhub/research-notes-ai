# Experiment: Embedding Model Comparison for RAG Retrieval

## Experiment Overview

This experiment evaluates different text embedding models for improving semantic search performance in a Retrieval-Augmented Generation (RAG) system.

Embedding models are responsible for converting text into numerical vectors that represent semantic meaning.

The quality of embeddings directly affects:

* Search accuracy
* Context retrieval
* RAG response quality

---

# Research Question

## Main Question

Which embedding model provides better semantic retrieval performance for a domain-specific RAG system?

---

## Sub Questions

1. How do different embedding models represent meaning?

2. Which model retrieves more relevant documents?

3. How does embedding dimension affect performance?

4. What is the trade-off between accuracy and computational cost?

---

# Background

Traditional keyword search depends on exact word matching.

Example:

Query:

```text id="m5q8xa"
How to fix authentication problem?
```

Keyword search looks for:

```text id="n8p3mz"
authentication
problem
fix
```

---

Semantic search understands meaning:

```text id="r4m7qa"
Login failure

=

Authentication issue
```

This capability comes from embedding models.

---

# Embedding Pipeline

Architecture:

```text id="p7m2qx"
                 Text Document

                       |

                       v

              Embedding Model

                       |

                       v

              Vector Representation

                       |

                       v

              Vector Database

                       |

                       v

              Similarity Search
```

---

# Models Selected for Experiment

## Model 1: all-MiniLM-L6-v2

Source:

Sentence Transformer

Characteristics:

* Lightweight
* Fast inference
* Good general performance

Use case:

* Small RAG systems
* Local AI assistants

---

## Model 2: BGE Embedding Model

Characteristics:

* Strong retrieval performance
* Optimized for search tasks

Use case:

* Enterprise search
* Knowledge retrieval

---

## Model 3: E5 Embedding Model

Characteristics:

* Instruction-aware embeddings
* Strong semantic understanding

Use case:

* Advanced RAG applications

---

# Experimental Setup

## Hardware

Example:

```text id="v6k9mx"
CPU:

Intel Processor

RAM:

16GB+

GPU:

Optional
```

---

## Dataset

Documents:

* AI research papers
* Software engineering notes
* Technical documentation
* GitHub README files

---

# Data Processing

Workflow:

```text id="q3m8za"
Documents

    |

Cleaning

    |

Chunking

    |

Embedding Generation

    |

Vector Storage
```

---

# Chunk Configuration

Experiment parameters:

```python id="u7m4qx"
Chunk Size:

512 tokens


Overlap:

64 tokens
```

Purpose:

Maintain enough context while keeping retrieval precise.

---

# Evaluation Method

## Query Dataset

Example questions:

```text id="x5p8mz"
1. What is Retrieval-Augmented Generation?

2. How do AI agents work?

3. Explain software maintenance using AI.

4. What is transformer architecture?
```

---

# Evaluation Metrics

## 1. Retrieval Accuracy

Measures:

Did the system retrieve the correct document?

---

## 2. Similarity Score

Higher score indicates stronger semantic relationship.

Example:

```text id="z9m3qa"
Query:

AI coding assistant


Result:

Code generation agent

Score:

0.87
```

---

## 3. Response Quality

Evaluation:

* Correctness
* Relevance
* Completeness

---

# Experimental Comparison

Example Result Table:

| Model            | Speed  | Accuracy  | Memory Usage |
| ---------------- | ------ | --------- | ------------ |
| all-MiniLM-L6-v2 | High   | Good      | Low          |
| BGE              | Medium | Very Good | Medium       |
| E5               | Medium | Excellent | Higher       |

---

# Observations

## all-MiniLM-L6-v2

Advantages:

* Fast
* Easy deployment
* Suitable for local applications

Limitations:

* Lower performance for complex queries

---

## BGE

Advantages:

* Better retrieval accuracy
* Strong semantic matching

Limitations:

* More computational requirements

---

## E5

Advantages:

* Strong understanding of query intent
* Good for advanced RAG systems

Limitations:

* Higher resource usage

---

# Example Retrieval Test

Query:

```text id="c6m8qa"
How can AI automatically fix software bugs?
```

Retrieved results:

```text id="h4p9mx"
1. Automated Program Repair

2. AI Software Maintenance

3. SWE-Agent Architecture
```

Expected:

Relevant software engineering documents.

---

# Result Analysis

Embedding quality impacts:

```text id="k8m4qa"
Better Embedding

        |

        v

Better Retrieval

        |

        v

Better Context

        |

        v

Better AI Answer
```

---

# Challenges

## Domain Knowledge Gap

General embedding models may not fully understand:

* Programming concepts
* Architecture patterns
* Technical terms

---

## Long Documents

Large documents require:

* Better chunking
* Hierarchical retrieval

---

# Future Improvements

## Domain-Specific Embeddings

Train embeddings using:

* Software repositories
* Research papers
* Technical documentation

---

## Hybrid Retrieval

Combine:

```text id="m2x7qa"
Vector Search

+

Keyword Search

+

Reranking
```

---

## Code Embeddings

Future experiment:

Compare:

* Text embeddings
* Code embeddings

for repository-level AI assistants.

---

# Research Contribution

This experiment demonstrates:

* Importance of embedding selection
* Effect of semantic representation
* Retrieval optimization for RAG systems

---

# Relation With AI Software Engineering

High-quality embeddings enable:

* Repository understanding
* Code search
* AI debugging agents
* Autonomous coding systems

Architecture:

```text id="s5m9qa"
Software Repository

        |

        v

Code Embedding

        |

        v

Vector Database

        |

        v

AI Coding Agent
```

---

# Future Research Direction

Potential research:

* Adaptive embedding selection
* Code-aware RAG
* Learning-based retrieval optimization
* Agentic retrieval systems

---

# Author

**Farid Ahmed**

Software Engineer | AI & Software Engineering Research Enthusiast
