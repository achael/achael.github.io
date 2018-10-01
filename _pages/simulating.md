---
layout: single
classes:
    - wide
    - landing
    - dark-theme
title: Black Hole Accretion Simulations
author_profile: true

header:
  overlay_image: /assets/images/banner.png
  image_description: "A simulation of Sgr A* as seen by the EHT at 230 GHz" 
  overlay_color: "#000"
  overlay_filter: "0.5"

gallery1:
  - url: /assets/images/sgrA.png
    image_path: /assets/images/sgrA.png
    alt: "Several simulated images of Sgr A*."
    title: "Images of Sgr A* from my simulations (Chael+ 2018a) with four different values of black hole spin and electron heating functions, as viewed by the EHT at 230 GHz."


gallery2:
  - url: /assets/images/m87_zoom.png
    image_path: /assets/images/m87_zoom.png
    alt: "Zooming in on the M87 jet"
    title: "Images of of the M87 jet at different frequencies from one of my MAD simulations (Chael+ 2018b). As the frequency increases, the brightest emission moves down the jet closer and closer to the black hole."


gallery3:
  - url: /assets/images/m87ims.png
    image_path: /assets/images/m87ims.png
    alt: "Images from my MAD simulations of M87 using damped turbulence (left) and magnetic reconnection (right)"
    title: "Images from my MAD simulations of M87 using damped turbulence (left) and magnetic reconnection (right) to heat electrons"

---

See my [Youtube channel](https://www.youtube.com/channel/UCXWFOi3uMYoUkRpYaz-wz8Q) for some movies of my simulations!

{% include video id="SiP1Yiifwz0" provider="youtube" %}

In the local universe, including the center of our own galaxy (Sgr A* ), most supermassive black holes are surrounded by hot, thick, and dim accretion disks. Many of these black holes, like the one in the  M87, launch relativistic jets powered by the rotational energy of the black hole itself. To understand the how plasma behaves in spacetime -- how it emits radiation, launches jets, and feeds the black hole -- one of our best tools are supercomputer simulations using the equations of General Relativistic Magnetohydrodynamics (GRMHD). 
 
{% include video id="WEFifaAGsRE" provider="youtube" %}

However, in the hot, weakly coupled plasmas around M87 and Sgr A* , protons and electrons are not in thermal equilibrium with each other. Most simulations assume thermodynamic equilibrium -- it is impossible to directly predict the electron temperature and radiation emitted from most simulations without making additional assumptions in post-processing. This makes predictions for the [images](/_pages/imaging) observed by the Event Horizon Telescope difficult.

{% include gallery id="gallery1" caption="Images of Sgr A* from my simulations [(Chael+ 2018a)](https://arxiv.org/abs/1804.06416) with four different values of black hole spin and electron heating functions, as viewed by the EHT at 230 GHz." %}{: .text-center}
{: .align-right}

In my research, I use the massively parallel code [KORAL](https://arxiv.org/abs/1605.03184) which moves beyond standard single-fluid GRMHD to a three-fluid approximation where electrons, ions, and photons exchange energy self-consistently. This method allows us to directly predict what the Event Horizon Telescope will see and how different models emit across the entire electromagnetic spectrum. In [Chael+ 2018a](https://arxiv.org/abs/1804.06416) I used two physical origins for electron heating in plasmas -- turbulence and magnetic reconnection -- to investigate how plasma microphysics changes the images and variability of Sgr A* at different frequencies. In Chael+ 2018b (in prep.), I applied the same method to M87's jet and determine that the observed characteristics are well explained by a Magnetically Arrested Disc model, where extreme magnetic fields on the black hole choke accretion. 

{% include gallery id="gallery2" caption="Images of of the M87 jet at different frequencies from one of my MAD simulations (Chael+ 2018b). As the frequency increases, the brightest emission moves down the jet closer and closer to the black hole." %}{: .text-center}
{: .align-right}

{% include gallery id="gallery3" caption="Images from my MAD simulations of M87 using damped turbulence (left) and magnetic reconnection (right) to heat electrons" %}{: .text-center}
{: .align-right}

In [Chael+ 2017](https://arxiv.org/abs/1704.05092), I made a major update to `KORAL` by adding a method to evolve a population of nonthermal electrons in space, time, and energy in
parallel with the thermal fluid. This represents the first time that _spectral_ resolution of electron
distributions is possible in grid-based accretion simulations. This method will open up new ground in understanding the nonthermal jet emission in M87 and nonthermal infrared and X-ray flares in Sgr A*.

{% include video id="0GH-C4Rmex0" provider="youtube" %}




 
