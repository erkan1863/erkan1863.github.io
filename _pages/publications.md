---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
{% include base_path %}


{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>

{% endif %}

<!-- {% include base_path %} -->
* **Bayram E.**, Liu S., Belabbas M.-A., Başar T., *Control Theoretic Approach to Fine-Tuning and Transfer Learning*. (SysDO24) [View on ArXiv](https://arxiv.org/abs/2404.11013)

* **Bayram E.**, Belabbas M. A., *Constructing Stochastic Matrices for Weighted Averaging in Gossip Networks*. (NecSys 25') [View on ArXiv](https://arxiv.org/abs/2502.19821)

* **Bayram E.**, Baştopçu M., Belabbas M.-A., Başar T., *Age of Coded Updates In Gossip Networks Under Memory and Memoryless Scheme*. [View on ArXiv](https://arxiv.org/abs/2410.19696)

* **Bayram E.**, Baştopçu M., Belabbas M.-A., Başar T., *Age of k-out-of-n Systems in a Gossip Network*. (Asilomar Conference 24') [View on IEEEXplore](https://ieeexplore.ieee.org/document/10942930)

* **Bayram E.**, Belabbas M.-A., Başar T., *Vector-Valued Gossip over $w$-Holonomic Networks*. (Under review) [View on ArXiv](https://arxiv.org/abs/2311.04455)

* Ergeneci M., **Bayram E.**, Carter D., Kosmas P., *A Novel Framework for Motion-Induced Artefact Cancellation in sEMG: Evaluation on EPL and Ninapro Datasets*. IEEE Sensors Journal, 24(15), 22610-22619. [View on IEEEXplore](https://ieeexplore.ieee.org/document/10542637)

* Ergeneci M., **Bayram E.**, Carter D., Kosmas P., *Attention-Enhanced Frequency-Split Convolution Block for sEMG Motion Classification: Experiments on Premier League and Ninapro Datasets*. IEEE Sensors Journal, 24(4), 4821-4830. [View on IEEEXplore](https://ieeexplore.ieee.org/abstract/document/10375923)

* Ergeneci M., **Bayram E.**, Carter D., Kosmas P., *sEMG Motion Classification Via Few-Shot Learning With Applications to Sports Science*. (preprint) [View on TechRxiv](https://www.techrxiv.org/articles/preprint/sEMG_Motion_Classification_Via_Few-Shot_Learning_With_Applications_To_Sports_Science/22577374)

 

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
