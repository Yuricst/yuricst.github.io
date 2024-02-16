---
title: 'Revisiting Optimal Control Theory'
date: 2023-09-09
permalink: /posts/2023/09/optimal-control/
tags:
  - cool posts
  - category1
  - category2
---

Revisiting optimal control theory for reference to my future self. 

Optimal Control Theory
======

Let the dynamics and the cost be given by

$$
\dot{\boldsymbol{x}}(t) = \boldsymbol{f} (\boldsymbol{x}(t), \boldsymbol{u}(t), t)
$$

$$
\mathcal{J}(\boldsymbol{u}) 
    = 
    h(\boldsymbol{x}(t_f), t_f) 
    +
    \int_{t_0}^{t_f} g(\boldsymbol{x}(t), \boldsymbol{u}(t), t) dt
$$

The Hamiltonian is given by

$$
\mathcal{H}(\boldsymbol{x}(t), \boldsymbol{u}(t), \boldsymbol{\lambda}(t), t)
    \triangleq 
    g(\boldsymbol{x}(t), \boldsymbol{u}(t), t)
    + \boldsymbol{\lambda}^T(t) \boldsymbol{f} (\boldsymbol{x}(t), \boldsymbol{u}(t), t)
$$

State constraint
------

Spacecraft trajectory problem
------
