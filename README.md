# Linguistic Audit of the Wolof-Labeled Subset (MURI-IT)

## Overview

This repository presents a methodological linguistic audit of the subset labeled as “Wolof” in the MURI-IT dataset.

The objective is to evaluate whether the linguistic labeling is consistent with the actual textual content using independent language identification models.

## Methodology

A hierarchical detection strategy was applied:

1. **Global multilingual detection** using fastText (176 languages)
2. Confidence-based filtering (τ = 0.7)
3. Specialized African language detection using AfroLID
4. Comparative triangulation analysis

## Key Findings

- 0% of instances were detected as Wolof with strong confidence using fastText.
- AfroLID classified 50.33% of ambiguous cases as Wolof, but with extremely low confidence scores (~0.0017).
- No robust Wolof signal was detected across models.

The results support the hypothesis of linguistic discordance between the labeling and actual content.

## Related Work

AfroLID selection was informed by prior evaluation:
https://github.com/MaDi-12/wolof-language-detection-eval

## Author

Marème Diop  
AI & Big Data Engineering
