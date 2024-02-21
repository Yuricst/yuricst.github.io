---
layout: splash
title: "Research Projects"
permalink: /research/
author_profile: true
excerpt: "List of research projects"
intro: 
  - excerpt: ''
feature_row_flp:
  - image_path: '../images/cflp_pmedian_sda.gif'
    alt: "pmediansda"
    title: "Facility Location Problem for Cislunar Space Domain Awareness"
    excerpt: '**Abstract:** Facility Location Problem for Space-Based Assets. 
    
    SUMMARY TEXT
    '

  - image_path: '../images/flp_allocation_D1m2000.png'
    alt: "osamdepotoflp"
    title: "Facility Location Problem for On-Orbit Servicing Depot"
    excerpt: '**Abstract:** Facility Location Problem for OSAM depot. '
    url: /research/flp_osam/
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_gnc:
  - image_path: '../images/opnav_rendering.png'
    alt: "opnavnrho"
    title: "Autonomous Optical Navigation on Near-Rectilinear Halo Orbit"
    excerpt: '
        The combined use of gravity assist, low-thrust propulsion, and manifold capture for interplanetary transfers is studied. This work makes use of the Sims-Flanagan transcription, incorporating parametrization of arrival to a manifold Poincaré section instead of a celestial body. 
        <br><br>
        **Related publication:** Y. Shimane, P. Miraldo, K. Berntorp, M. Greiff, P. Elango, and A. Weiss, “High-Fidelity Simulation of Horizon-Based Optical Navigation with Open-Source Software,” in 74th International Astronautical Congress, 2023. Available: [https://www.merl.com/publications/docs/TR2023-128.pdf](https://www.merl.com/publications/docs/TR2023-128.pdf)
    '

feature_row_astrodynamics:
  - image_path: '../images/galt_manifold.png'
    alt: "galt"
    title: "Gravity-Assist Low-Thrust Trajectory Design"
    excerpt: '
        The combined use of gravity assist, low-thrust propulsion, and manifold capture for interplanetary transfers is studied. This work makes use of the Sims-Flanagan transcription, incorporating parametrization of arrival to a manifold Poincaré section instead of a celestial body. 
        <br><br>
        **Related publication:** Shimane, Y., & Ho, K. (2022). Gravity‑Assist Low‑Thrust Inter‑System Trajectory Design with Manifold Captures. The Journal of the Astronautical Sciences. [https://doi.org/10.1007/s40295-022-00319-x](https://doi.org/10.1007/s40295-022-00319-x)
    '
    url: /research/galt/
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

## Facility Location Problems

{% include feature_row id="feature_row_flp" type="left" %}

## Guidance, Navigation, and Control (GNC)

{% include feature_row id="feature_row_gnc" type="left" %}

## Astrodynamics and Trajectory Design

{% include feature_row id="feature_row_astrodynamics" type="left" %}