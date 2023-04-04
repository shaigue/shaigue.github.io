---
layout: post
title:  "Concurrent Games with Multiple Topologies"
permalink: /concurrent-games-with-multiple-topologies
date:   2022-11-01 
image: "static/images/concurrent_games_with_multiple_topologies.PNG"
---
<center><img src="{{ page.image }}" width="30%" height="auto"></center>
<br>
In my master's thesis, we studied Nash Equilibria in concurrent games with multiple topologies. A [game](https://en.wikipedia.org/wiki/Game_theory) is a mathematical model that represents interactions among self-interested agents. In computer science, games are used to model systems that are composed of different components, each component free to choose its actions and aims to optimize its objective.

[Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium) is a stable state of a game where no player can change their behavior to improve their outcome. Different algorithms exist for finding Nash Equilibria in various types of games. However, the problem of finding Nash Equilibria in games with incomplete information is undecidable, meaning that there is no algorithm for finding them in general.

In our work, we examined a limited type of partial information, called multi-topology games, where players can play one of several different games (topologies), but they don’t know at the start of the game exactly which one they are in. We showed that this problem is decidable and presented an algorithm for solving it.

Our work was presented at [The 33rd International Conference on Concurrency Theory (CONCUR 2022)](https://concur2022.mimuw.edu.pl/). You can read the full paper on [arxiv](https://arxiv.org/abs/2207.02596) and check out the [slides](static/pdfs/Concurrent Games with Multiple Topologies slides.pdf).
