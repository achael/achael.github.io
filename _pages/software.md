---
layout: single
classes:
    - wide
    - landing
    - dark-theme
title: Software
author_profile: true

header:
  overlay_image: /assets/images/banner.png
  image_description: "A simulation of Sgr A* as seen by the EHT at 230 GHz" 
  overlay_color: "#000"
  overlay_filter: "0.5"

---
### `ehtim`

I wrote `ehtim`  (`eht-imaging`) as a python framework for implementing regularized maximum likelihood imaging methods on EHT data. It has evolved into a flexible environment for manipulating, simulating, analyzing, and imaging interferometric data and is a workhorse of the EHT's data analysis pipeline.

`ehtim` has so far been used in over 50 peer reviewed publications. If you reconstruct images from visibilities and are interested in trying out some new methods beyond CLEAN, give `ehtim` a shot! The code is on [GitHub](https://github.com/achael/eht-imaging), and the documentation is [here](https://achael.github.io/eht-imaging/).

### `kgeo`

[`kgeo`](https://github.com/achael/kgeo) is a lightweight Python code for generating null geodesics in the Kerr spacetime around a supermassive black hole. It can create fully polarized black hole images from simple emission models. It can also create videos like the one below illustrating the trajectories of photons that make up a black hole image. 

{% include video id="PYC2tdmDU1w" provider="youtube" %}

### `KORAL`

I maintain the two-temperature, radiative GRMHD C code [`KORAL`](https://github.com/achael/koral_lite) originally written by Aleksander Sadowski. I use `KORAL` to investigate the effects of adding new physics [like the spectral evolution of nonthermal electrons](https://arxiv.org/abs/1704.05092) or [more accurately modeling high-magnetization plasma](https://arxiv.org/abs/2404.01471) to standard GRMHD simulations of the EHT's target black hole sources. I am currently working on porting KORAL to a new, GPU-capable code. 

<br/><br/>

