---
title: CaLMFlow
subtitle: "Volterra Flow Matching using Causal Language Models"
summary: We frame flow matching as a Volterra integral equation and apply causal language models to solve it.
date: 2024-10-08
cardimage: CaLMFlow.png
featureimage: CaLMFlow.png
caption: Overview of the CaLMFlow framework. CaLMFlow takes as input textual conditions and flows and generates the next time point for the flows. The textual condition is tokenized and embedded using the LLM tokenizer and embedding layer while the conditional flows are transformed into spatial-temporal tokens using a learned projection. If multiple conditional flows are input simultaneously, the tokens are ordered by flow, space, and then time. The LLM applies causal language modeling and generates the next time point for each flow.}
---
## Abstract
We introduce CaLMFlow (Causal Language Models for Flow Matching), a novel framework that casts flow matching as a Volterra integral equation (VIE), leveraging the power of large language models (LLMs) for continuous data generation. CaLMFlow enables the direct application of LLMs to learn complex flows by formulating flow matching as a sequence modeling task, bridging discrete language modeling and continuous generative modeling. Our method implements tokenization across space and time, thereby solving a VIE over these domains. This approach enables efficient handling of high-dimensional data and outperforms ODE solver-dependent methods like conditional flow matching (CFM). We demonstrate CaLMFlow's effectiveness on synthetic and real-world data, including single-cell perturbation response prediction, showcasing its ability to incorporate textual context and generalize to unseen conditions. Our results highlight LLM-driven flow matching as a promising paradigm in generative modeling, offering improved scalability, flexibility, and context-awareness.

## Authors
- **Sizhuang He** (Co-first author)
- Daniel Levine (Co-first author)
- Ivan Vrkic
- Marco Bressana
- David Zhang
- Syed Rizvi
- Yangtian Zhang
- Emanuele Zappala
- David van Dijk

## Cite this paper
S. He, D. Levine, I. Vrkic, M. Bressana, D. Zhang, S. Rizvi, Y. Zhang, E. Zappala, and D. van Dijk, *CaLMFlow: Volterra Flow Matching using Causal Language Models*, [arXiv:2410.05292](https://arxiv.org/pdf/2410.05292)