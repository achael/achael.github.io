---
layout: single
classes:
    - wide
    - landing
    - dark-theme
title: Imaging Black Holes with the EHT
author_profile: true

header:
  overlay_image: /assets/images/banner.png
  image_description: "A simulation of Sgr A* as seen by the EHT at 230 GHz" 
  overlay_color: "#000"
  overlay_filter: "0.5"

gallery0:
  - url: /assets/images/eht_banner.jpg
    image_path: /assets/images/eht_banner.jpg
    alt: "M87 in 2017"
    title: "The first resolved images of a black hole taken by the EHT in 2017"

gallery1:
  - url: /assets/images/EHT.jpg
    image_path: /assets/images/EHT_small.jpg
    alt: "EHT 2017"
    title: "The stations of the Event Horizon Telescope"

gallery2:
  - url: /assets/images/sim_and_reconstruct.png
    image_path: /assets/images/sim_and_reconstruct.png
    alt: "Simulated EHT image of M87 and reconstruction with eht-imaging."
    title: "(Left) an image of M87 at 230 GHz from one of my simulations. (Right) the image reconstructed with eht-imaging from realistic simulated data similar to the EHT's observations in 2017. The circle at the lower right represents the EHT's effective resolution"

gallery3:
  - url: /assets/images/hltau.png
    image_path: /assets/images/hltau.png
    alt: "Reconstruction of an ALMA image of HL Tau using traditional CLEAN vs eht-imaging."
    title: "(Left) an image of the protoplanetary disk in HL Tau from Band 7, 0.87 mm ALMA observations using the traditional CLEAN algorithm. (Right) the image reconstructed from the same data with eht-imaging using an imaging algorithm robust to errors in amplitude and phase calibration (Chael+ 2018)."

---
{% include gallery id="gallery0" caption="The first resolved images of a black hole taken by the EHT in 2017" %}{: .text-center}
{: .align-right}

{% include gallery id="gallery1" caption="The stations of the Event Horizon Telescope" %}{: .align-right}

The [EHT](http://eventhorizontelescope.org/) is globe-spanning [VLBI](https://en.wikipedia.org/wiki/Very-long-baseline_interferometry) array that observes the nearest supermassive black holes in 
<a href="https://en.wikipedia.org/wiki/Sagittarius_A*">Sgr A* </a> 
and [M87](https://en.wikipedia.org/wiki/Messier_87) at 1.3 mm wavelength. After years of preparation the EHT observed Sgr A* and M87 with telescopes around the world in the spring of 2017 and 2018 ([see pictures from the observations](https://eventhorizontelescope.org/galleries/2017-observations)).

In April 2019, we published the results of our observations of M87; the first images of a supermassive black hole with resolution on event-horizon scales ([Read the papers](https://iopscience.iop.org/journal/2041-8205/page/Focus_on_EHT)).

By correlating the recorded electric field measured simultaneously at telescopes around the world, the EHT can effectively _synthesize_ the resolving power of an Earth-sized telescope with an angular resolution of about 10 _microarcseconds_ (1 / 360000000<sup>th</sup> of a degree!)

Both because EHT measurements are sparse and because absolute phase calibration at millimeter wavelengths is impossible, recovering an image from EHT observations is a difficult and ill-posed problem. Images must be _reconstructed_ using algorithms that find the best-fit images to data under a (hopefully minimal) set of additional assumptions about the source structure.

{% include gallery id="gallery2" caption="(Left) an image of M87 at 230 GHz from one of my simulations. (Right) the image reconstructed with `ehtim` from realistic simulated data similar to the EHT's observations in 2017. The circle at the lower right represents the EHT's effective resolution" %}{: .text-center}
{: .align-right}


As a leading member of the EHT's Imaging Working Group, I develop new Bayesian imaging methods that push the EHT's imaging capabilities to higher fidelity and resolution. I have developed algorithms that bypass traditional self-calibration both for total intensity [(Chael+ 2018)](https://arxiv.org/abs/1803.07088) and polarization [(Chael+ 2016)](https://arxiv.org/abs/1605.06156). 

My software library [`ehtim`](https://github.com/achael/eht-imaging) has become a standard tool across the collaboration for imaging and analyzing EHT data ([click here](/_pages/software) for more information). The techniques and software I've developed for the EHT have wide application across radio and optical interferomerty, and we are currently exploring their application on [LOFAR](http://www.lofar.org/) and [ALMA](http://www.almaobservatory.org/en/home/) datasets. 

{% include gallery id="gallery3" caption="(Left) an [image](https://arxiv.org/pdf/1503.02649.pdf) of the protoplanetary disk in HL Tau from Band 7, 0.87 mm ALMA observations using the traditional CLEAN algorithm. (Right) the image reconstructed from the same data with `ehtim` using an imaging algorithm robust to errors in amplitude and phase calibration [(Chael+  2018)](https://arxiv.org/abs/1803.07088)."
 %}{: .text-center}
{: .align-right}

I work closely on developing imaging algorithms and applying them to EHT observations with [Katie Bouman](https://people.csail.mit.edu/klbouman/index.html), [Kazu Akiyama](http://kazuakiyama.github.io/pages/aboutme.html), and [Michael Johnson](http://www.scintillatingastronomy.com/).




