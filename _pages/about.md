---
permalink: /
title: "Biography"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

**Actively looking for full-time software engineer opportunies starting August 2025**

Hi everyone, I am currently a 5th-year Computer Science Ph.D. student at Georgia Tech. My advisor is [Vivek Sarkar](https://vsarkar.cc.gatech.edu/). Prior to my Ph.D. journey, I earned my bachelor degree from [Washington University in St. Louis](https://washu.edu/) in December 2019.

My research area is dynamic HPC/Parallel program analysis. My Ph.D. thesis focused on understanding, detecting and fixing data races in parallel programs. I have developed several dynamic debugging tools for [OpenMP](https://www.openmp.org/) and [HClib](https://github.com/habanero-rice/hclib) programs. Additionaly, my reserach achieves theoretical breakthroughs and utilizes Large Language Model in industrial settings. 

Email: fjin35 at gatech.edu

Research problems
=================
I am proud that my research pushes the boundary of human's understanding of data races and program behavior.

**Determinism**: given the same input, how do we guarantee the programs will return the same output? How do we even define "same" here? In my [ECOOP](https://feiyangjin.github.io/publication/ecoop) paper, I give the formal definition of determinism for task-parallel programs with promises, and prove that data race freedom guarantees determinism for such program. 

**Happens-before relation**: task A happens before task B if and only if in all possible scheduing of the program, task A has to finish before task B starts. 

**Concurrent access**: if two tasks does not have happens-before relationship between them, we say they can happen in parallel (or concurrently). The exact order will be determined by the runtime. In one schedule, task A may happen before task B. In the other schedule, it may be the other way around. 

**Data race**: if two tasks concurrently access the same memory location, and at least one of them perform a write, we define this as a data race. Data race is notorious because it makes program non-deterministic. Imagine task A writes 5 to variable x, and task B writes 3 to it. When the program ends, we have no idea what the value of x will be: 5 or 3, that's a question. 

**Dynamic race detection**: To detect data races while running the program, we use compiler to "instrument" each read and write in the program. Instrument means we insert a check function after each read and write. This is done on the IR level.
When the program is running, the check function records each read and write, and see if a previous access causes a data race with the current access. \
My [ECOOP](https://feiyangjin.github.io/publication/ecoop) paper designs a new race detection algorithm and evalutes the implementation of it. It is sound and precise: meaning it will not report non-existing race or miss any races. 