---
title: Research
date: 2026-09-15 00:00:00
academia: true
---

## Research

### BoolXLLM: LLM-Assisted Explainability for Boolean Models

**Du Cheng, Serdar Kadioglu, and Xin Wang. 2026.**  
*BoolXLLM: LLM-Assisted Explainability for Boolean Models.* arXiv preprint.  
[arXiv:2605.12139](https://arxiv.org/abs/2605.12139)

Boolean rule models are attractive for explainable AI because their decisions can be represented as logical formulas rather than opaque model weights. But even when the model is formally interpretable, the resulting rules can still be hard for non-technical stakeholders to understand or use. BoolXLLM addresses this gap by combining Boolean rule learning with large language models.

The framework augments BoolXAI with LLM assistance at three points in the pipeline: selecting semantically meaningful features, recommending useful thresholds for discretizing numerical variables, and translating learned Boolean rules into natural-language explanations. This keeps the core model faithful and symbolic while using language models to improve usability, accessibility, and communication.

This work reflects a practical direction for explainable AI: instead of replacing interpretable models with black-box systems, it uses LLMs as an interface layer around transparent models. The result is an explainability workflow that can support both global explanations of model behavior and local explanations for individual predictions.

### Read-Write-Learn: Self-Learning for Handwriting Recognition

**Adrian Boteanu, Du Cheng, and Serdar Kadioglu. 2023.**  
*Read-Write-Learn: Self-Learning for Handwriting Recognition.* DocEng '23, Article 21, 1-4.  
[DOI: 10.1145/3573128.3609343](https://doi.org/10.1145/3573128.3609343)

Handwriting recognition often depends on large labeled datasets, but that assumption breaks down for historical documents, specialized collections, and lower-resource languages where annotation is expensive or scarce. This paper explores a self-learning loop for handwriting recognition built around three steps: read, write, and learn.

The core idea is to let a recognition model identify examples it is likely reading correctly, use a language model to help select reliable text, generate additional handwriting samples in a matching style, and then fine-tune the recognizer on the expanded data. Instead of treating synthetic data as generic augmentation, the framework uses generated examples to adapt to the specific writing style present in the target documents.

What I like about this work is its practical framing: the method is designed for settings where more labels are not easy to obtain. It also connects recognition, generation, and language modeling into one training loop, which is a useful pattern for many low-supervision AI problems.

### Bias Mitigation in Recommender Systems to Improve Diversity

**Du Cheng, Doruk Kilitcioglu, and Serdar Kadioglu. 2022.**  
*Bias Mitigation in Recommender Systems to Improve Diversity.* CIKM 2022 Workshops, EvalRS Workshop.  
[PDF](https://ceur-ws.org/Vol-3318/short6.pdf)

Recommendation systems are often optimized around engagement and ranking metrics, but those metrics can hide uneven performance across user groups or item groups. This paper studies bias mitigation for recommenders in the context of the CIKM 2022 EvalRS Challenge, where systems were evaluated with a broader set of quality and diversity metrics.

The work starts from an implicit-feedback collaborative filtering baseline using Alternating Least Squares, then explores two ways to improve recommendation behavior across protected groups. The first is activity-based averaging, where models trained for user activity groups are combined with an overall model. The second is post-processing with equalized odds calibration, adapted from binary fairness methods to the recommendation setting by binarizing item scores and reordering recommendations.

The broader lesson is that recommender quality is multi-objective. Accuracy, hit rate, diversity, and group-level behavior can move in different directions, so evaluation has to make those tradeoffs visible. The paper is especially interesting as a practical example of adapting fairness tooling to recommender systems, where the output is not a single binary decision but a ranked list of items.

### Three-dimensional orientation of compact high velocity clouds

**F. Heitsch, B. Bartell, S. E. Clark, J. E. G. Peek, D. Cheng, and M. Putman. 2016.**  
*Three-dimensional orientation of compact high velocity clouds.* Monthly Notices of the Royal Astronomical Society: Letters, 462(1), L46-L50.  
[DOI: 10.1093/mnrasl/slw124](https://doi.org/10.1093/mnrasl/slw124)

This paper presents a proof-of-concept method for estimating the inclination angle of compact high velocity clouds, defined as the angle between a cloud's trajectory and the observer's line of sight. The method uses cloud morphology and kinematics, calibrated with numerical simulations, to connect observable position-velocity asymmetries with the cloud's three-dimensional orientation. 

