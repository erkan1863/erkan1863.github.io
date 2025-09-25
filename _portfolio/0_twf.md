---
title: "Control Theory for Learning"
excerpt: "Using control theory for robust fine-tuning <br/><img src='/images/flow_single_control.png'>"
collection: portfolio
---

In this project, we are integrating nonlinear control theory approach into the learning theory.

In [Control Theoretic Approach to Fine-Tuning and Transfer Learning](https://erkan1863.github.io/publication/2024-04-17-TuningWithoutForgetting), we introduce here the concept of tuning without forgetting. We develop an iterative algorithm to tune the control or system parameters when the training set expands, whereby points already memorized remain so, and new training samples are additional memorized.

<br/><img src='/images/twf.png'>


* In the limit of a large number of layers, a deep neural network can be modeled as a controlled differential equation, where the control function u act as the network parameters. 

* Fine-tuning is a technique in which a pre-trained model is further trained on a new dataset (tuning data) to adapt it to a specific task while retaining knowledge from the original dataset. A {\em control-theoretic} approach provides a natural framework for this problem.

* A common fine-tuning method is the penalty method, which penalizes deviations between pre-trained weights (u_0) and tuned weights ($\tilde u$). However, this method can reduce accuracy, as there are no guarantee that weights close to u_0 will effectively accommodate the new data. Consequently, the pre-trained weights $u_0$ initially map x_i to y_i, but after tuning, they may ``forget'' this data.

* Our method, Tuning without Forgetting (TwF), finds new weights $u^*$ that are tuned to the new data while preserving performance on the pre-trained data. To that end, established conditions under which the space of controls (weights) that retains the pre-training data forms an infinite-dimensional connected Banach submanifold. We then optimize the weights via a descent method on this manifold, ensuring tuning without forgetting. 

* In our numerical experiments, we compare TwF with the penalty method across varying sizes of training and tuning datasets.


In [Geometric Foundations of Tuning without Forgetting in Neural ODEs](https://erkan1863.github.io/publication/2025-09-02-GeoFoundationsTwF), we introduced the principle of Tuning without Forgetting (TwF) for sequential training of neural ODEs, where training samples are added iteratively and parameters are updated within the subspace of control functions that preserves the end-point mapping at previously learned samples on the manifold of output labels in the first-order approximation sense. In this letter, we prove that this parameter subspace forms a Banach submanifold of finite codimension under nonsingular controls, and we characterize its tangent space. This reveals that TwF corresponds to a continuation/deformation of the control function along the tangent space of this Banach submanifold, providing a theoretical foundation for its mapping-preserving (not forgetting) during the sequential training exactly, beyond first-order approximation.


In [Control Disturbance Rejection in Neural ODEs](https://erkan1863.github.io/publication/2025-09-24-control_disturbance_node), we propose an iterative training algorithm for Neural ODEs that provides models resilient to control (parameter) disturbances. The method builds on our earlier work Tuning without Forgetting-and similarly introduces training points sequentially, and updates the parameters on new data within the space of parameters that do not decrease performance on the previously learned training points-with the key difference that, inspired by the concept of flat minima, we solve a minimax problem for a non-convex non-concave functional over an infinite-dimensional control space.



