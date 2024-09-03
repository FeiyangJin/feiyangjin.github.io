---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download my CV](http://feiyangjin.github.io/files/FeiyangJin_CV_2024.pdf)
======

Education
======
* Ph.D in Computer Science, Georgia Institute of Technology, 2025 (expected)
* B.S. in Computer Science, Washington University in St. Louis, 2019

Work experience
======
* Google
  * Summser 2024
  * Ph.D. Software Engineer Intern, Google Cloud, Flex (Resource & Infrastructure Optimization Technology)
  * Project:
    * Implement a framework to characterize job network traffic through different profiling techniques. This flow has enabled the comparison between different profiles to decide the best for different applications 
    * Develop a methodology to pinpoint profiles that best predict future job behavior
    * Enhance resource utilization for resource management tools through the implemented methodology


* Uber
  * Summer 2023
  * Ph.D. Software Engineer Intern, Infrastructure Team, Programming System Group
  * Project:
    * Design, implement and evaluate a closed-loop application that uses LLM (Large Language Model) to repair Golang programs with concurrency bugs 
    * Learn and use internal infrastructure and AST (Abstract syntax tree) for Golang program compilation, analysis, deployment and bug report 
    * Fix data races found and reported to the internal issue database
  
Skills
======
* Advanced: C++
* Intermediate: OpenMP, Python, SQL, LLVM
* Basic: C, MATLAB, Java, R, Kokkos, Golang

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
<!-- Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul> -->
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Paper reviewer: VIVEKFEST 2024, SPLASH Workshop
