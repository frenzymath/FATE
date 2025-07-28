# FATE  
The **FATE (Formal Algebra Theorem Evaluation)** benchmarks.  

## Overview  
This collection contains three benchmarks in abstract algebra and commutative algebra:  
- **FATE-M** (150 exercises)  
- **FATE-H** (100 exercises)  
- **FATE-X** (100 exercises)  

All exercises are formalized in Lean.  

## Mathematical Level  

The problems in these benchmarks are sourced from:  
- Undergraduate and graduate textbooks,  
- Final exams and PhD qualifying exams,  
- Research literature.  

Broadly speaking, the three benchmarks have progressively increasing difficulty:  
- **FATE-M** consists primarily of standard textbook exercises (basic level),  
- **FATE-H** contains challenging problems from abstract/commutative algebra final exams,  
- **FATE-X** includes problems at PhD qualifying exam level and beyond.  

## Benchmark Structure  

Each Lean file in every benchmark contains:  
- One fully formalized statement,  
- A single `sorry`,  
- Appropriate open namespaces at the beginning,  
- Natural language annotations preceding the statement.  

Key differences:  
- **FATE-M** and **FATE-H**: No extra definitions are included,  
- **FATE-X**: Minimal dependent definitions formalized before the statement. 

## Usage Recommendation  
For users' convenience, we provide a PDF file and a JSON file for each benchmark to make reading and usage easier.

We strongly recommend AGAINST combining these benchmarks due to their:  
- Significantly different difficulty levels,  
- Distinct formalization characteristics. 

## Problem Distribution

<figure>
  <img src="https://raw.githubusercontent.com/frenzymath/FATE/main/assets/FATE-H&X-sunburst.svg" width="600" alt="Mathematical Categorical Distribution of FATE-H and FATE-X">
  <figcaption>
    Figure 1. Mathematical Categorical Distribution of FATE-H and FATE-X
  </figcaption>
</figure>

## Additional Information  
The FATE-M benchmark is a refactored version of the benchmark referenced in:  
[**REAL-Prover: Retrieval-Augmented Lean Prover for Mathematical Reasoning**](https://arxiv.org/abs/2505.20613)  

