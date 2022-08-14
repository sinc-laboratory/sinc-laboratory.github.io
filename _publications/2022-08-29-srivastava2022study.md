---
layout: default-publication
title: "A Study on Robustness to Perturbations for Representations of Environmental Sound"
collection: publications
permalink: /publications/2022-08-29-srivastava2022study
abstract: "Audio applications involving environmental sound analysis increasingly use general-purpose audio representations, also known as embeddings, for transfer learning. Recently, Holistic Evaluation of Audio Representations (HEAR) evaluated twenty-nine embedding models on nineteen diverse tasks. However, the evaluation&apos;s effectiveness depends on the variation already captured within a given dataset. Therefore, for a given data domain, it is unclear how the representations would be affected by the variations caused by myriad microphones&apos; range and acoustic conditions - commonly known as channel effects. We aim to extend HEAR to evaluate invariance to channel effects in this work. To accomplish this, we imitate channel effects by injecting perturbations to the audio signal and measure the shift in the new (perturbed) embeddings with three distance measures, making the evaluation domain-dependent but not task-dependent. Combined with the downstream performance, it helps us make a more informed prediction of how robust the embeddings are to the channel effects. We evaluate two embeddings - YAMNet, and OpenL3 on monophonic (UrbanSound8K) and polyphonic (SONYC-UST) urban datasets. We show that one distance measure does not suffice in such task-independent evaluation. Although Frechet Audio Distance (FAD) correlates with the trend of the performance drop in the downstream task most accurately, we show that we need to study FAD in conjunction with the other distances to get a clear understanding of the overall effect of the perturbation. In terms of the embedding performance, we find OpenL$^3$ to be more robust than YAMNet, which aligns with the HEAR evaluation."
date: 2022-08-29
venue: 'European Signal Processig Conference'
venue_short: 'EUSIPCO'
paperurl: '/files/srivastava2022study.pdf'
image: '/assets/images/srivastava2022study.png'
imagewidth: 75.0
presentation: '/files/srivastava2022study_presentation.pdf'
categories: 
  - Environmental Machine Listening
  - Audio Representation Learning
citation: 'Srivastava, S., Wu, H., Rulff, J., Fuentes, M., Cartwright, M., Silva, C., Arora, A., Bello, J.P. A Study on Robustness to Perturbations for Representations of Environmental Sound. In <i>Proceedings of the European Signal Processing Conference (EUSIPCO)</i>, 2022.'
---