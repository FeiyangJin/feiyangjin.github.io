---
title: "Visualizing Correctness Issues in OpenMP Programs"
collection: publications
category: workshops
permalink: /publication/iwomp
excerpt: 'This work builds a data race visualizer for OpenMP programs'
date: 2024-09-22
venue: 'The 20th International Workshop on OpenMP (IWOMP 2024)'
paperurl: 'http://feiyangjin.github.io/files/iwomp.pdf'
citation: 'Feiyang Jin, Alan Tao, Lechen Yu, Vivek Sarkar. Visualizing Correctness Issues in OpenMP Programs. In 20th International Workshop on OpenMP (IWOMP 2024).'
---

Past work on OpenMP program visualization has mainly centered on performance analysis. This paper explores how the visualization of computation graphs assists programmers in debugging issues related to program correctness. The motivation is twofold. First, researchers widely use computation graphs to analyze dynamic program behavior. Second, most past work focused on visualizing performance bottlenecks rather than correctness issues. 

This paper's contributions are as follows. First, we introduce techniques for building computation graphs using the OpenMP Tools Interface (OMPT). **Second, we present a computation graph visualizer for OpenMP programs built upon these techniques.** The visualizer specifically highlights data races as the correctness issue under study. A key innovation is a novel OMPT callback to precisely model host-device data movements, an unprecedented feature among existing callbacks. **Finally, the paper includes an empirical study of the performance and effectiveness of our prototype.** The evaluation demonstrates that our graph builder introduces minimal overhead when integrated with state-of-the-art race detectors.
We also conducted a user study involving a control group and an experimental group. The results show that our visualization greatly aids programmers in understanding and debugging data races. Beyond our main contribution, which focuses on data races, we also integrate host-device data movement in the visualization. This serves as a first step toward visualizing data mapping issues. To the best of our knowledge, our work is the first to explore understanding of correctness issues in OpenMP programs through interactive visualization of computation graphs.