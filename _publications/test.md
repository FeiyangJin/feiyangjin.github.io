---
title: "Early notice: GenAI-based Datarace Fix for Real-World Golang Programs"
collection: publications
category: workshops
permalink: /publication/test
excerpt: 'This work uses Large Language Model to fix data races'
date: 2023-12-15
venue: 'Machine Learning for Systems 2023'
paperurl: 'http://feiyangjin.github.io/files/mlsys.pdf'
citation: 'Jin, F., Zhang, Z., Barik, R., Korlam, G., & Chabbi, M. Early notice: GenAI-based Datarace Fix for Real-World Golang Programs.'
---

Data race detection has been a subject of extensive research for decades; the practical deployment of race detectors has also become increasingly commonplace in industrial settings. However, the focus has mainly been on the detection aspect, with relatively little attention directed toward the challenging task of autonomously repairing programs with data races. This discrepancy is understandable given the inherent complexities of fixing the data race and the substantial engineering efforts required to integrate fixes into existing workflows.

**In this paper, we introduce a novel closed-loop application that harnesses the power of Generative AI to fix data races automatically.** Our early experiments involving this application within Uber's internal codebase have yielded promising results. The evaluation results suggest a bright future for integrating this application into Uber's infrastructure, potentially revolutionizing how data races are handled in large-scale software development environments.