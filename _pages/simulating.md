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


gallery4:
  - url: /assets/images/m87_proposal-1.png
    image_path: /assets/images/m87_proposal-1.png
    alt: "The inner shadow of M87 in my simulation images"
    title: "The inner shadow of M87 in my simulation images"
---

See my [Youtube channel](https://www.youtube.com/channel/UCySmvivwH2TekzO67quZ9fg/featured) for some movies of my simulations!

{% include video id="NF2dcg7XM0k" provider="youtube" %}

In the local universe, including the center of our own galaxy (Sgr A* ), most supermassive black holes are surrounded by hot, thick, and dim accretion disks. Many of these black holes, like the one in the  M87, launch relativistic jets powered by the rotational energy of the black hole itself. To understand how plasma behaves in spacetime -- how it emits radiation, launches jets, and feeds the black hole -- one of our best tools is supercomputer simulations using the equations of General Relativistic Magnetohydrodynamics (GRMHD). 
 
{% include video id="MSkemJnNL54" provider="youtube" %}

Unfortunately, in the hot, weakly coupled plasmas around M87 and Sgr A* , protons and electrons are not in thermal equilibrium with each other. Since most simulations assume thermodynamic equilibrium  it is impossible to directly predict the radiation emitted from most simulations without making additional assumptions in post-processing. This makes predictions for the [images](/_pages/imaging) observed by the Event Horizon Telescope difficult.

{% include gallery id="gallery1" caption="Images of Sgr A* from my simulations [(Chael+ 2018a)](https://arxiv.org/abs/1804.06416) with four different values of black hole spin and electron heating functions, as viewed by the EHT at 230 GHz." %}{: .text-center}
{: .align-right}

In my research, I use the massively parallel code [KORAL](https://arxiv.org/abs/1605.03184) which moves beyond standard single-fluid GRMHD to a three-fluid approximation where electrons, ions, and photons exchange energy self-consistently. This method allows us to directly predict what the Event Horizon Telescope will see and how different models emit across the entire electromagnetic spectrum. In [Chael+ 2018a](https://arxiv.org/abs/1804.06416) I tested two physical mechanisms for electron heating in plasmas -- turbulence and magnetic reconnection -- to investigate how plasma microphysics changes the images and variability of Sgr A* at different frequencies. 

In [Chael+ 2019](https://arxiv.org/abs/1810.01983), I applied the same method to M87's jet and determined that the observed characteristics are well explained by a Magnetically Arrested Disc model, where extreme magnetic fields on the black hole choke accretion. In 2021, I was a co-coordinator of the [paper](https://iopscience.iop.org/article/10.3847/2041-8213/abe4de) EHT's first polarimetric images of M87; we found that EHT polarimetric observations also strongly favor a magnetically arrested accretion flow. 

{% include gallery id="gallery2" caption="Images of of the M87 jet at different frequencies from one of my MAD simulations (Chael+ 2018b). As the frequency increases, the brightest emission moves down the jet closer and closer to the black hole." %}{: .text-center}
{: .align-right}

{% include gallery id="gallery3" caption="230 GHz images from my MAD simulations of M87 using damped turbulence (left) and magnetic reconnection (right) to heat electrons" %}{: .text-center}
{: .align-right}

In [Chael+ 2021](https://arxiv.org/abs/2106.00683), I used my simulation images to examine the role of the ``inner shadow'' in black hole images. In MAD simulations, the 230 GHz emission is nearly equatorial and extends to the black hole event horizon. As a result, the lensed image of the horizon itself is visible as a deep brightness depression in these images, but only at very high dynamic range, as strong gravitational redshift causes emission to fade to zero at the horizon. Measuring the size and shape of this brightness depression in addition to the photon ring of multiply lensed images can provide additional constraints on the black hole metric from future EHT observations. 

{% include gallery id="gallery4" caption="230 GHz images from my MAD simulations of M87 using  magnetic reconnection (center) with the position of the photon ring and black hole inner shadow indicated. The left image shows a simulated EHT reconstruction of this simulation snapshot, and the right image shows the snapshot in a gamma color scale, where faint features are more visible" %}{: .text-center}
{: .align-right}

In [Chael+ 2017](https://arxiv.org/abs/1704.05092), I updated to `KORAL` to evolve a population of nonthermal electrons in space, time, and energy in
parallel with the thermal fluid. This represents the first time that _spectral_ resolution of electron
distributions is possible in grid-based accretion simulations. My current work is focused on extending this method to realistic presciptions for electron acceleration and running the first global 3D simulations of black hole accretion including the spectral evolution of electrons. This method will open up new ground in understanding the nonthermal jet emission in M87 and nonthermal infrared and X-ray flares in Sgr A*.

{% include video id="i4E6mnnZvIk" provider="youtube" %}




 
