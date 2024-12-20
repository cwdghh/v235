---
title: 'Provably Robust DPO: Aligning Language Models with Noisy Feedback'
openreview: yhpDKSw7yA
abstract: Learning from preference-based feedback has recently gained traction as
  a promising approach to align language models with human interests. While these
  aligned generative models have demonstrated impressive capabilities across various
  tasks, their dependence on high-quality human preference data poses a bottleneck
  in practical applications. Specifically, noisy (incorrect and ambiguous) preference
  pairs in the dataset might restrict the language models from capturing human intent
  accurately. While practitioners have recently proposed heuristics to mitigate the
  effect of noisy preferences, a complete theoretical understanding of their workings
  remain elusive. In this work, we aim to bridge this gap by introducing a general
  framework for policy optimization in the presence of random preference flips. We
  focus on the direct preference optimization (DPO) algorithm in particular since
  it assumes that preferences adhere to the Bradley-Terry-Luce (BTL) model, raising
  concerns about the impact of noisy data on the learned policy. We design a novel
  loss function, which de-bias the effect of noise on average, making a policy trained
  by minimizing that loss robust to the noise. Under log-linear parameterization of
  the policy class and assuming good feature coverage of the SFT policy, we prove
  that the sub-optimality gap of the proposed robust DPO (rDPO) policy compared to
  the optimal policy is of the order $O(\frac{1}{1-2\epsilon}\sqrt{\frac{d}{n}})$,
  where $\epsilon < 1/2$ is flip rate of labels, $d$ is policy parameter dimension
  and $n$ is size of dataset. Our experiments on IMDb sentiment generation and Anthropic’s
  helpful-harmless dataset shows that rDPO is robust to noise in preference labels
  compared to vanilla DPO and other heuristics proposed by practitioners.
layout: inproceedings
series: Proceedings of Machine Learning Research
publisher: PMLR
issn: 2640-3498
id: ray-chowdhury24a
month: 0
tex_title: 'Provably Robust {DPO}: Aligning Language Models with Noisy Feedback'
firstpage: 42258
lastpage: 42274
page: 42258-42274
order: 42258
cycles: false
bibtex_author: Ray Chowdhury, Sayak and Kini, Anush and Natarajan, Nagarajan
author:
- given: Sayak
  family: Ray Chowdhury
- given: Anush
  family: Kini
- given: Nagarajan
  family: Natarajan
date: 2024-07-08
address:
container-title: Proceedings of the 41st International Conference on Machine Learning
volume: '235'
genre: inproceedings
issued:
  date-parts:
  - 2024
  - 7
  - 8
pdf: https://raw.githubusercontent.com/mlresearch/v235/main/assets/ray-chowdhury24a/ray-chowdhury24a.pdf
extras: []
# Format based on Martin Fenner's citeproc: https://blog.front-matter.io/posts/citeproc-yaml-for-bibliographies/
---
