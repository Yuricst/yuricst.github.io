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
feature_row_logistics:
  - image_path: '../images/cflp_pmedian_sda.gif'
    alt: "telescopeJSSP"
    title: "Multi-Sensor Tasking for Ground-Based Telescopes via Job-Shop Scheduling Problem"
    excerpt: '
    The short-term telescope tasking problem consists of rapidly constructing a sensor-tasking schedule for observing resident space objects (RSO) passing overhead. Due to the short-term prediction horizon necessitated by this application, motion of RSOs can be assumed to be exactly known, making the prolbem deterministic. We derive a job-shop-scheduling problem for both single and multi-telescope sensor-tasking scenarios. 
    <br><br>
    **Related publication:** Y. Shimane, N. Gollins, and K. Ho, “Multi-Sensor Tasking for Ground-Based Space Situational Awareness via Job-Shop Scheduling Problem,” in AAS/AIAA Space Flight Mechanics Meeting, 2025. Available: [Conference server](https://s3.amazonaws.com/amz.xcdsystem.com/A464D031-C624-C138-7D0E208E29BC4EDD_abstract_File24835/PreprintPaperUploadPDF_321_0103063552.pdf)
    '
    url: /research/telescope_tasking/
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: '../images/cflp_pmedian_sda.gif'
    alt: "pmediansda"
    title: "Time-Expanded p-Median Problem for Cislunar Space Situational Awareness"
    excerpt: '
    This work formulates a novel time-expanded p-Median problem to design space-based observer constellations for Cislunar Space Situational Awareness (CSSA). We also derive a Lagrangean relaxation-based algorithm to rapidly obtain near-optimal solutions. 
    <br><br>
    **Related publication:** Y. Shimane, K. Tomita, and K. Ho, “Cislunar Constellation Design for Space Situational Awareness with Time-Expanded p-Median Problem,” 2024, [Online]. Available: [http://arxiv.org/abs/2408.06238](http://arxiv.org/abs/2408.06238)
    '
    url: /research/TEpMP_ssa/
    btn_label: "Read More"
    btn_class: "btn--primary"

  - image_path: '../images/flp_allocation_D1m2000.png'
    alt: "osamdepotoflp"
    title: "Facility Location Problem for On-Orbit Servicing Depot"
    excerpt: '
    This work formulates a facility location problem for on-orbit servicing depot in Medium Earth Orbit (MEO), considering low-thrust round-trip servicers. 
    <br><br>
    **Related publication:** Y. Shimane, N. Gollins, and K. Ho, “Orbital Facility Location Problem for Satellite Constellation Servicing Depots,” J. Spacecr. Rockets, pp. 1–18, Mar. 2024, doi: 10.2514/1.A35691. [https://arc.aiaa.org/doi/full/10.2514/1.A35691](https://arc.aiaa.org/doi/full/10.2514/1.A35691)
    '
    url: /research/flp_osam/
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_gnc:
  - image_path: '../images/PhaseSOCP.png'
    alt: "sklpo"
    title: "Optimization-Based Station-Keeping on Libration Point Orbits"
    excerpt: '
        **With:** Mitsubishi Electric Research Laboratories
        <br><br>
        In this work, an optimization-based station-keeping algorithm for colinear libration point orbits (LPO) based on the xz-plane crossing control technique is conceived. The optimization problem is cast as a sequential second-order cone pro- gram and incorporates an explicit constraint on the perilune pass epoch to en- sure the steered trajectory follows the reference baseline without deviating in phase. The resulting formulation has easily interpretable tuning parameters that may be obtained directly from mission requirements. The algorithm is demonstrated through Monte-Carlo simulations on the Gateway’s Near Rectilinear Halo Orbit (NRHO) in the full-ephemeris dynamics with realistic error models.
        <br><br>
        **Related publication:** Y. Shimane, K. Ho, and A. Weiss “Optimization-Based Phase-Constrained Station-Keeping Control on Libration Point Orbit,” in AAS/AIAA Astrodynamics Specialist Conference, 2024. Available: [https://www.merl.com/publications/docs/TR2024-109.pdf](https://www.merl.com/publications/docs/TR2024-109.pdf)
    '

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

# 1. Space Logistics

{% include feature_row id="feature_row_logistics" %}

# 2. Guidance, Navigation, and Control (GNC)

{% include feature_row id="feature_row_gnc" %}

# 3. Astrodynamics and Trajectory Design

{% include feature_row id="feature_row_astrodynamics" %}