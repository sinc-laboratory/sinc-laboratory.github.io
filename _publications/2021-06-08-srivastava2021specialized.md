---
layout: default-publication
title: "Specialized Embedding Approximation for Edge Intelligence: A Case Study in Urban Sound Classification"
collection: publications
permalink: /publications/2021-06-08-srivastava2021specialized
abstract: "Embedding models that encode semantic information into low-dimensional vector representations are useful in various machine learning tasks with limited training data. However, these models are typically too large to support inference in small edge devices, which motivates training of smaller yet comparably predictive student embedding models through knowledge distillation (KD). While knowledge distillation traditionally uses the teacher&#8217;s original training dataset to train the student, we hypothesize that using a dataset similar to the student&#8217;s target domain allows for better compression and training efficiency for the said domain, at the cost of reduced generality across other (non-pertinent) domains. Hence, we introduce <i>Specialized Embedding Approximation</i> (SEA) to train a student featurizer to approximate the teacher&apos;s embedding manifold for a given target domain. We demonstrate the feasibility of SEA in the context of acoustic event classification for urban noise monitoring and show that leveraging a dataset related to this target domain not only improves the baseline performance of the original embedding model but also yields competitive students with &gt; 1 order of magnitude lesser storage and activation memory. We further investigate the impact of using random and informed sampling techniques for dimensionality reduction in SEA."
date: 2021-06-08
venue: 'IEEE International Conference on Acoustics, Speech and Signal Processing'
venue_short: 'ICASSP'
paperurl: '/files/srivastava2021specialized.pdf'
image: '/assets/images/specialized_embedding.png'
imagewidth: 75.0
presentation: '/files/srivastava2021specialized_presentation.pdf'
poster: '/files/srivastava2021specialized_poster.pdf'
code: 'https://github.com/ksangeeta2429/edgel3'
codename: 'EdgeL3 python package'
categories: 
  - Environmental Machine Listening
  - Audio Representation Learning
citation: 'Srivastava, S., Roy, D., Cartwright, M., Bello, J.P., Arora, A. Specialized Embedding Approximation for Edge Intelligence: A Case Study in Urban Sound Classification.  In <i>Proceedings of the IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)</i>, 2021.'
---