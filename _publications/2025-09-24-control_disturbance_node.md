---
title: "Control Disturbance Rejection in Neural ODEs"
collection: publications
permalink: /publication/2025-09-24-control_disturbance_node
# excerpt: 'This paper is about fixing template issue #693.'
date: 2024-09-24
venue: 'To appear at CDC 2025'
paperurl: 'https://arxiv.org/abs/2509.18034'
citation: 'Geometric Foundations of Tuning without Forgetting in Neural ODEs
E Bayram, MA Belabbas, T Başar, in 2025 IEEE 64th Annual Conference on Decision and Control (CDC), IEEE, 2025.'
---

In this paper, we propose an iterative training algorithm for Neural ODEs that provides models resilient to control (parameter) disturbances. The method builds on our earlier work Tuning without Forgetting-and similarly introduces training points sequentially, and updates the parameters on new data within the space of parameters that do not decrease performance on the previously learned training points-with the key difference that, inspired by the concept of flat minima, we solve a minimax problem for a non-convex non-concave functional over an infinite-dimensional control space. We develop a projected gradient descent algorithm on the space of parameters that admits the structure of an infinite-dimensional Banach subspace. We show through simulations that this formulation enables the model to effectively learn new data points and gain robustness against control disturbance.
