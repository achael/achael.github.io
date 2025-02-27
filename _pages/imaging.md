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
{% include gallery id="gallery0" caption="The first resolved images of a black hole taken by the EHT in 2017 ([Paper IV](https://iopscience.iop.org/article/10.3847/2041-8213/ab0e85), Fig. 15)" %}{: .text-center}
{: .align-right}

{% include gallery id="gallery1" caption="The stations of the Event Horizon Telescope" %}{: .align-right}

The [EHT](http://eventhorizontelescope.org/) is globe-spanning [VLBI](https://en.wikipedia.org/wiki/Very-long-baseline_interferometry) array that observes the nearest supermassive black holes in 
<a href="https://en.wikipedia.org/wiki/Sagittarius_A*">Sgr A* </a> 
and [M87](https://en.wikipedia.org/wiki/Messier_87) at 1.3 mm wavelength. After years of preparation the EHT observed Sgr A* and M87 with telescopes around the world in the spring of 2017 and 2018 ([see pictures from the observations](https://eventhorizontelescope.org/galleries/2017-observations)).


By correlating the recorded electric field measured simultaneously at telescopes around the world, the EHT can effectively _synthesize_ the resolving power of an Earth-sized telescope with an angular resolution of about 10 _microarcseconds_ (1 / 360000000<sup>th</sup> of a degree!)
Both because EHT measurements are sparse and because absolute phase calibration at millimeter wavelengths is impossible, recovering an image from EHT observations is a difficult and ill-posed problem. Images must be _reconstructed_ using algorithms that find the best-fit images to data under a (hopefully minimal) set of additional assumptions about the source structure.

{% include gallery id="gallery2" caption="(Left) an image of M87 at 230 GHz from one of my simulations. (Right) the image reconstructed with `ehtim` from realistic simulated data similar to the EHT's observations in 2017. The circle at the lower right represents the EHT's effective resolution" %}{: .text-center}
{: .align-right}

### New Techniques for Imaging in Interferometry 
As a leading member of the EHT's imaging team, I develop new imaging methods that push the EHT's imaging capabilities to higher fidelity and resolution. I have developed algorithms that bypass traditional self-calibration both for total intensity [(Chael+ 2018)](https://arxiv.org/abs/1803.07088) and polarization [(Chael+ 2016)](https://arxiv.org/abs/1605.06156). In [Chael+ 2023](https://iopscience.iop.org/article/10.3847/1538-4357/acb7e4), I extended the regularized maximum likelihood imaging technique to recover multi-frequency imgages and spectral index maps from simulated EHT data and real VLBA and ALMA datasets. 

### The First Black Hole Images 
In April 2019, we published the results of our observations of M87; the first images of a supermassive black hole with resolution on event-horizon scales ([read the papers](https://iopscience.iop.org/journal/2041-8205/page/Focus_on_EHT)). After devoting significant effort to overcoming the rapid variability in the Galactic Center observations, we published corresponding [images of Sgr A*](https://iopscience.iop.org/journal/2041-8205/page/Focus_on_First_Sgr_A_Results) in 2022. After these initial images were released, I co-led projects to image and interpret [linear](https://iopscience.iop.org/article/10.3847/2041-8213/abe71d) and [circular](https://iopscience.iop.org/article/10.3847/2041-8213/acff70) polarization data from the EHT, which directly constrain the magnetic field structure near the event horizon.

### `eht-imaging`: a community tool 
My software library [`eht-imaging`](https://github.com/achael/eht-imaging) has become a standard tool across the collaboration for imaging and analyzing EHT data ([click here](/_pages/software) for more information). `eht-imaging` has been essential for producing the first EHT images at micro-arcsecond resolution of M87 in [total intensity](https://iopscience.iop.org/article/10.3847/2041-8213/ab0e85) and [polarization](https://iopscience.iop.org/article/10.3847/2041-8213/abe71d), [Sgr A*](https://iopscience.iop.org/article/10.3847/2041-8213/ac6429),  [Centaurus A](https://www.nature.com/articles/s41550-021-01417-w),  [3C279](https://www.aanda.org/articles/aa/full_html/2020/08/aa37493-20/aa37493-20.html),  and [J1924-2914](https://iopscience.iop.org/article/10.3847/1538-4357/ac7a40). `eht-imaging` is used for data analysis in interferometry beyond the EHT, including to make high-resolution images from [RadioAstron](https://arxiv.org/pdf/2311.01861) the [VLBA](https://arxiv.org/pdf/2401.03603) the [GVA](https://arxiv.org/pdf/2408.09069) and [VGOS Geodesy observations](https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2020JB021238).

{% include gallery id="gallery3" caption="(Left) an [image](https://arxiv.org/pdf/1503.02649.pdf) of the protoplanetary disk in HL Tau from Band 7, 0.87 mm ALMA observations using the traditional CLEAN algorithm. (Right) the image reconstructed from the same data with `ehtim` using an imaging algorithm robust to errors in amplitude and phase calibration [(Chael+  2018)](https://arxiv.org/abs/1803.07088)."
 %}{: .text-center}
{: .align-right}

<br/><br/>



