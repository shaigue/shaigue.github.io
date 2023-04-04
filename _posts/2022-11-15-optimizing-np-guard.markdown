---
layout: post
title:  "Optimizing NP-Guard"
permalink: /optimizing-np-guard
date:   2022-11-15 
image: "/static/images/optimizing-np-guard.gif"
# categories: jekyll update
---
<center><img src="{{ page.image }}" width="30%" height="auto"></center>
<br>
As part of my summer internship at [IBM Research Israel](https://research.ibm.com/labs/haifa/), I worked on a project that was part of a larger open-source tool called [NP-Guard](https://np-guard.github.io/). The tool is designed to help developers write more secure Kubernetes network policies and automate the error-prone process. NP-Guard achieves this by converting Kubernetes network policies and specifications into mixed string and integer product sets, and different tool functions are mapped to set operations such as emptiness check and computing the union or intersection between two sets. The tool's set operations are computed using an in-house built engine.

My main focus during this project was on optimizing the tool's performance by modifying the in-house engine. I explored two options to achieve this goal. The first option was to use the [Z3 theorem prover](https://github.com/Z3Prover/z3) instead of the in-house engine. The second option was to modify the in-house engine to use a more compact DAG-based (Directed Acyclic Graph) data structure instead of a tree-based data structure to represent the sets, which would allow for more efficient computation. The implementation of the new data structure was inspired by [BDDs](https://dl.acm.org/doi/10.1145/123186.123222).

You can find more details about my project in the [slides](/static/pdfs/network_config_analyzer_optimization_slides.pdf), and you can learn more about the larger NP-Guard tool on its [website](https://np-guard.github.io/) or its [GitHub repository](https://github.com/np-guard).
