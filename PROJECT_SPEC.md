# Industrial Material Classification

## Motivation

This project was inspired by a real-world material classification and data quality challenge observed in an industrial environment.

The original challenge motivated the exploration of how machine learning could support the classification of noisy material descriptions and determine when predictions are reliable enough for automation.

This is an independent portfolio project. It uses synthetic data, an original taxonomy, and independently designed rules. 

## Objective

Build an end-to-end machine learning system that classifies noisy industrial material descriptions into a standardized taxonomy and determines when predictions are reliable enough for automatic classification.

The system should support both new material records and historical unclassified records.

## Core Question

How much of a material catalog can be safely automated at different precision thresholds?


## Input

A free-text industrial material description.

The dataset may contain:

- Abbreviations
- Typos
- Word reordering
- Missing attributes
- Mixed languages
- Unit variations
- Punctuation variations
- Casing variations
- Combined noise

## Output

The system should provide:

- Predicted category
- Top 3 predictions
- Confidence score
- Automation decision
- Model explanation

## Automation Decisions

### AUTO

High-confidence predictions that meet the selected precision criteria can be automatically classified.

### REVIEW

Medium-confidence predictions are sent for human review.

### ABSTAIN

Low-confidence predictions are not automatically classified and require manual intervention.

## Evaluation

The project will evaluate the trade-off between model precision and automation coverage.

Key metrics include:

- Precision
- Recall
- F1-score
- Automation Coverage
- Calibration
- Abstention Rate
- Performance under different noise conditions