---
title: "Control Theory for Learning"
excerpt: "Using control theory for robust fine-tuning <br/><img src='/images/flow_single_control.png'>"
collection: portfolio
---

In this project, we are integrating nonlinear control theory approach into the learning theory.

In [Control Theoretic Approach to Fine-Tuning and Transfer Learning](https://erkan1863.github.io/publication/2024-04-17-TuningWithoutForgetting), we introduce here the concept of tuning without forgetting. We develop an iterative algorithm to tune the control or system parameters when the training set expands, whereby points already memorized remain so, and new training samples are additional memorized.

<br/><img src='/images/twf.png'>


* In the limit of a large number of layers, a deep neural network can be modeled as a controlled differential equation, where the control function $u$ act as the network parameters. 

* Fine-tuning is a technique in which a pre-trained model is further trained on a new dataset (tuning data) to adapt it to a specific task while retaining knowledge from the original dataset. A {\em control-theoretic} approach provides a natural framework for this problem.

* A common fine-tuning method is the penalty method, which penalizes deviations between pre-trained weights (u_0) and tuned weights ($\tilde u$). However, this method can reduce accuracy, as there are no guarantee that weights close to u_0 will effectively accommodate the new data. Consequently, the pre-trained weights $u_0$ initially map x_i to y_i, but after tuning, they may ``forget'' this data.

* Our method, Tuning without Forgetting (TwF), finds new weights $u^*$ that are tuned to the new data while preserving performance on the pre-trained data. To that end, established conditions under which the space of controls (weights) that retains the pre-training data forms an infinite-dimensional connected Banach submanifold. We then optimize the weights via a descent method on this manifold, ensuring tuning without forgetting. 

* In our numerical experiments, we compare TwF with the penalty method across varying sizes of training and tuning datasets.



