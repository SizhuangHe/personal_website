---
title: Iterative Methods
subtitle: "Improving neural networks"
summary: Many existing deep learning model adopts the notion of iterations, such as diffusion models, AlphaFold etc., either explicitly or implicitly. We put this under the framework of operator learning and understand it using functional analysis.
date: 2023-10-04
cardimage: IterativeMethods.png
featureimage: IterativeMethods.png
caption: Overview of iterative framework. (A) Popular architectures which incorporate iterative components in their framework. (B) Convergence behavior of an iterative solver. (C) Behavior of iterative solver converging to a fixed point in the data manifold.
---

In this work, we try to lay some theoretical foundation work for deep neural networks.

We frame deep neural networks as operators, between functional spaces, with fixed points, representing desired solutions and develop a theoretical framework based on iterative methods in operator learning. 

We demonstrate that many popular deep learning models, such as diffusion models, AlphaFold and autoregressive models, empirically adopted, either explicitly or implicitly, such iterative methods to boost model performance. We conduct a series of experiments to demonstrate benefits of iterations on model performance. 

We also introduce Picard Iteration Graph Neural Network (PIGN) as a further demonstration of how iterations boost model performance.

Please see [our paper](https://arxiv.org/pdf/2310.01618.pdf) for more details.