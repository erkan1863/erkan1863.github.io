---
title: "Age of k-out-of-n Systems on a Gossip Network"
collection: publications
permalink: /publication/2024-02-18-age_k_n_TSS_on_gossip
# excerpt: ''
date: 2024-02-18
venue: '58th Asilomar Conference on Signal, Systems and Computer 24'
paperurl: 'https://ieeexplore.ieee.org/document/10942930'
citation: 'Age of k-out-of-n Systems on a Gossip Network
E Bayram, M Bastopcu, MA Belabbas, T Başar - arXiv preprint arXiv:2402.11462, 2024'
---

We consider information update systems on a gossip network, which consists of a single source and n receiver nodes. The source encrypts the information into n distinct keys with version stamps, sending a unique key to each node. For decoding the information in a k-out-of-n system, each receiver node requires at least k+1 different keys with the same version, shared over peer-to-peer connections. Each node determines k based on a given function, ensuring that as k increases, the precision of the decoded information also increases. We consider two different schemes: a memory scheme (in which the nodes keep the source's current and previous encrypted messages) and a memoryless scheme (in which the nodes are allowed to only keep the source's current message). We measure the ''timeliness'' of information updates by using the k-keys version age of information. Our work focuses on determining closed-form expressions for the time average age of information in a heterogeneous random graph under both with memory and memoryless schemes.