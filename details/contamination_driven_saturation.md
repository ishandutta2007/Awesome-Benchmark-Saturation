# Contamination-Driven Saturation (Data Bleed)

## Overview
Contamination-Driven Saturation represents a critical data engineering failure where test data leaks into the model's pre-training corpus.

## Mechanism & Details
Since modern models train on web-scale crawls, public benchmarks are frequently indexed and trained on. This results in the model memorizing answers, giving the illusion of reasoning capability.

## Conceptual Workflow
```mermaid
flowchart TD
    A[Public Benchmarks Published] --> B[Inadvertent Web Scraping]
    B --> C[Pre-Training Dataset Contamination]
    C --> D[Zero-Shot Reasoning Illusion]
    D --> E[Memorized Metric Saturation]
```

## Key Characteristics
- **Dynamic Adaptability**: Evaluated continuously against changing distributions.
- **Robustness Target**: Addresses edge-cases and structural failures.
- **Evaluation Paradigm**: Shifting from static validation to interactive systems.

[Back to Main README](../README.md)
