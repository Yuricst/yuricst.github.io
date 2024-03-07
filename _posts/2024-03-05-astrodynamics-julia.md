---
title: 'Astrodynamics and the Julia language'
date: 2024-03-05
permalink: /posts/2024/03/blog-post-1/
tags:
  - astrodynamics
  - julia
  - programming
---

My research is almost entirely based on writing code, so I end up spending quite a bit of time working with different programming languages, developing code for all sorts of simulations, piping different tools, etc. 
I don't necessarily believe that [Julia](https://julialang.org/) is the best language for *all* purposes - but I do believe that it is a great language, particularly for research in optimization theory/astrodynamics (comme par hasard!).

Research coding requires a lot of trial and error, especially since I tend to get new ideas or discover pitfalls while I implement things. Occasionally, I want to be able to have lazy syntax (e.g. a cheeky double for-loop) without having to pay (too much) with performance. And for these purposes, Julia is great. 
Of course, there are also the well-discussed Julia perks - its speed (thank you JIT), ease of parallelization (<3), and capability to write mathematical notation-like code, to name a few. 

That is not to say Julia is good for everything; there are situations where things just have to be implemented in C/C++; if I need to pipe multiple software, I think python is still easier to work with; finally, there are some (I am sure many more, but at least some that I occasionally work with) that are best explored with other languages, namely: machine learning (beyond some simple regression-style NN tasks), global optimization (the pagmo/pygmo libraries are just too good, and I personally feel that the Julia metaheuristics options are not as advanced). 

Anyway, for (research in) Astrodynamics, I do think Julia can be an attractive option!

- dynamic language that is fast! (numba/cython is nice, but can be limiting)
- [`DifferentialEquations.jl`](https://github.com/SciML/DifferentialEquations.jl) is rich in capabilities (type of algorithms, customizability, parallelism paradigms...)
- there is a SPICE wrapper - [`SPICE.jl`](https://github.com/JuliaAstro/SPICE.jl)
- [`JuMP.jl`](https://github.com/jump-dev/JuMP.jl) provides good support for solving LP/MILP/QP/CP etc. within a modeling language setting

Meanwhile, drawbacks that I personally felt using Julia is: 

- Lack of widely-used black-box NLP solver (or wrapper to solver like SNOPT/IPOPT) where variables can be passed as a vector of floats rather than defining as a "variable" type (i.e. *not* a modeling language)

Below is a few packages for astrodynamics routines that I have used as building blocks to some of my research projects. 


## Packages

Available:

- [`AstrodynamicsBase.jl`](https://github.com/Yuricst/AstrodynamicsBase.jl) - basic astrodynamics routines for coordinate transformations, handling two-body orbital elements, defining astrodynamics constants, solving Kepler's problem, etc.
- [`Lambert.jl`](https://github.com/Yuricst/Lambert.jl) - native Lambert solver, implementing Dario Izzo's revised algorithm. Also implements the MGA-1DSM model for high-thrust, gravity-assist interplanetary trajectory optimization.
- [`R3BP.jl`](https://github.com/Yuricst/R3BP.jl/) - routines for restricted three-body problems (CR3BP, BCR4BP)
- [`FullEphemerisPropagator.jl`](https://github.com/Yuricst/FullEphemerisPropagator.jl) - full-ephemeris spacecraft state propagation library, building on top of `DifferentialEquations.jl`. 


*Coming soon!*

- [Navigation.jl]
- [QLaw.jl]