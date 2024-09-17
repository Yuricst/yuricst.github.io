---
layout: splash
title: "Research Projects"
permalink: /research/
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.0"
  overlay_image: '../images/banner/setouchi1.JPG'
  caption: "(c) Yuri Shimane / Setouchi, Japan"
intro: 
  - excerpt: ''
feature_row_flp:
  - image_path: '../images/cflp_pmedian_sda.gif'
    alt: "pmediansda"
    title: "Facility Location Problem for Cislunar Space Situational Awareness"
    excerpt: '
    This work proposes a facility location problem framework for designing satellite constellations to provide Cislunar Space Situational Awareness (CSSA). The problem seeks to find the optimal locations of space-based observers to monitor a user-defined region of cislunar space, represented by a finite set of targets with potentially time-varying observation requirements. The optimization problem is posed as a time-expanded facility location problem (FLP); unlike a traditional FLP that focuses on assigning facilities to clients, the proposed formulation focuses on assigning observers to specific pointing directions from a discretized set. To aid with the solving process of the resulting large-scale binary linear program, a Lagrangean method (LM) based on constraint relaxation and custom heuristics is provided. The performance of the proposed formulation and method is demonstrated with several case studies that obtained CSSA constellations for monitoring the lunar sphere of influence, the cislunar Cone of Shame, and a transit window for low-energy transfers located in the Earth-Moon L2 neck region. The proposed problem formulation, along with the LM, is demonstrated to enable a fast assessment of near-optimal CSSA constellations.
    <br><br>
    **Related publication:** Y. Shimane, K. Tomita, and K. Ho, “Cislunar Constellation Design for Space Situational Awareness with Time-Expanded Facility Location Problem,” 2024, [Online]. Available: [http://arxiv.org/abs/2408.06238](http://arxiv.org/abs/2408.06238)
    '

  - image_path: '../images/flp_allocation_D1m2000.png'
    alt: "osamdepotoflp"
    title: "Facility Location Problem for On-Orbit Servicing Depot"
    excerpt: '
    This work proposes an adaptation of the Facility Location Problem for the optimal placement
    of on-orbit servicing depots for satellite constellations in high-altitude orbit. The high-altitude regime, such as Medium Earth Orbit (MEO), is a unique dynamical environment where lowthrust propulsion systems can provide the necessary thrust to conduct plane-change maneuvers between the various orbital planes of the constellation. As such, on-orbit servicing architectures involving servicer spacecraft that conduct round-trips between servicing depots and the client satellites of the constellation may be conceived. To this end, a new orbital facility location problem formulation is proposed based on binary linear programming, in which the costs of operating and allocating the facility(ies) to satellites are optimized in terms of the sum of the Equivalent Mass to Low Earth Orbit (EMLEO). 
    <br><br>
    **Related publication:** Y. Shimane, N. Gollins, and K. Ho, “Orbital Facility Location Problem for Satellite Constellation Servicing Depots,” J. Spacecr. Rockets, pp. 1–18, Mar. 2024, doi: 10.2514/1.A35691. [https://arc.aiaa.org/doi/full/10.2514/1.A35691](https://arc.aiaa.org/doi/full/10.2514/1.A35691)
    '
    url: /research/flp_osam/
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_gnc:
  - image_path: '../images/cam_opnav_14days0001-2016_compressed.gif'
    alt: "opnavnrho"
    title: "Autonomous Optical Navigation on Near-Rectilinear Halo Orbit"
    excerpt: '
        **With:** Mitsubishi Electric Research Laboratories
        <br><br>
        Autonomous navigation capability in cislunar space is critical for the safe operation of both uncrewed and crewed spacecraft. This project explores the use of horizon-based optical navigation to autonomously navigate and conduct station-keeping for a spacecraft on the 9:2 Near-Rectilinear Halo Orbit (NRHO) in the full-ephemeris model. 
        <br><br>
        **Related publication:** Y. Shimane, P. Miraldo, K. Berntorp, M. Greiff, P. Elango, and A. Weiss, “High-Fidelity Simulation of Horizon-Based Optical Navigation with Open-Source Software,” in 74th International Astronautical Congress, 2023. Available: [https://www.merl.com/publications/docs/TR2023-128.pdf](https://www.merl.com/publications/docs/TR2023-128.pdf)
    '

feature_row_astrodynamics:
  - image_path: '../images/gtoc12_density.png'
    alt: "galt"
    title: "12th Global Trajectory Optimisation Competition"
    excerpt: '
        **With:** ESA ACT&Friends
        <br><br>
        We competed in the 12th GTOC competition and ended up 4th place overall!
        <br><br>
        **Related publication:** (coming soon!)
    '

  - image_path: '../images/galt_manifold.png'
    alt: "galt"
    title: "Gravity-Assist Low-Thrust Trajectory Design"
    excerpt: '
        The combined use of gravity assist, low-thrust propulsion, and manifold capture for interplanetary transfers is studied. This work makes use of the Sims-Flanagan transcription, incorporating parametrization of arrival to a manifold Poincaré section instead of a celestial body. 
        <br><br>
        **Related publication:** Y. Shimane and K. Ho, “Gravity‑Assist Low‑Thrust Inter‑System Trajectory Design with Manifold Captures,” J. Astronaut. Sci., 2022. [https://doi.org/10.1007/s40295-022-00319-x](https://doi.org/10.1007/s40295-022-00319-x)
    '
    url: /research/galt/
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: '../images/gtoc11_mothers_overview.png'
    alt: "galt"
    title: "11th Global Trajectory Optimisation Competition"
    excerpt: '
        **With:** ESA ACT&Friends
        <br><br>
        We competed in the 11th GTOC competition and ended up 2nd place overall!
        <br><br>
        **Related publication:** M. Märtens, D. Izzo, E. Blazquez, M. von Looz, P. Gomez, A. Mergy, G. Accdiarini, C.H. Yam, J. Hernando-Ayuso, Y. Shimane, “The fellowship of the Dyson ring: ACT&Friends’ results and methods for GTOC 11,” Acta Astronaut., no. February, 2022. [https://doi.org/10.1016/j.actaastro.2022.06.025](https://doi.org/10.1016/j.actaastro.2022.06.025)
    '
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
---

{% include feature_row id="intro" type="center" %}

# 1. In-Space Asset Design and Optimization

{% include feature_row id="feature_row_flp" %}

# 2. Guidance, Navigation, and Control (GNC)

{% include feature_row id="feature_row_gnc" %}

# 3. Astrodynamics and Trajectory Design

{% include feature_row id="feature_row_astrodynamics" %}