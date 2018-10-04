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

I wrote `ehtim`  (`eht-imaging`) as a python framework for implementing regularized maximum likelihood imaging methods on EHT data. In the last two years, it has evolved into a flexible environment for manipulating, simulating, analyzing, and imaging interferometric data and is a workhorse of the EHT's data analysis pipeline.

`ehtim` has already been used in 10 peer reviewed publications and is currently being used and developed by at least one group outside the EHT collaboration. If you reconstruct images from visibilities and are interested in trying out some new methods beyond CLEAN, give `ehtim` a shot! The code is on [GitHub](https://github.com/achael/eht-imaging), and the documentation is [here](https://achael.github.io/eht-imaging/).

### `KORAL`

I maintain the two-temperature, radiative GRMHD C code `KORAL` written by Aleksander Sadowski. In addition to adding new physics [like the spectral evolution of nonthermal electrons](https://arxiv.org/abs/1704.05092), I am also in the middle of refreshing the code, enhancing its performance and streamlining its structure to make future development easier. I hope to share a new, open-source version of `KORAL` on GitHub soon!
