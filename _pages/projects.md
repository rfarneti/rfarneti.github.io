---
title: "Projects"
permalink: /projects/
author_profile: true

---

{% include base_path %}

## Current and Past Projects

### The Southern Ocean Freshwater Input from Antarctica ([SOFIA](https://sofiamip.github.io/)) Initiative
___
The Southern Ocean Freshwater Input from Antarctica (SOFIA) Initiative aims to improve our understanding of the simulated response to Antarctic freshwater input, and in particular the model uncertainty.
The initiative has developed an experimental protocol and is engaging with modelling groups from around the world to run this common set of experiments using a variety of coupled climate and ocean-only models. Data from this international multi-model ensemble is openly shared for analysis, and is being synthesized into a series of publications by SOFIA participants.
The initiative was started by the CliC/CLIVAR/SCAR Southern Ocean Regional Panel, is endorsed as a CLIVAR task team, and has been submitted as a community MIP to CMIP7.

<p align="left">
  <img src="/images/SOFIA.png" alt="SOFIA" style="width:15%;
  text-align:left"/>
<figcaption>   </figcaption>
</p>

([Swart et al. (2023)](https://doi.org/10.5194/gmd-16-7289-2023)) 

### Flux-anomaly-forced model intercomparison project ([FAFMIP](http://www.fafmip.org/))
___
FAFMIP is an atmosphere-ocean general circulation model intercomparison project of CMIP6, initiated in 2016. Its purpose is to investigate the model spread in AOGCM projections of ocean climate change forced by CO2 increase. This spread is due to the different AOGCMs' differing simulations of regional ocean density and circulation changes, especially in high latitudes and the North Atlantic.

[Ocean-only FAFMIP]( https://doi.org/10.1029/2019MS002027) uses a novel design of ocean general circulation model (OGCM) experiments to investigate the ocean's response to surface buoyancy and momentum flux perturbations without atmosphere-ocean feedbacks.

([Navarro-Labastida, R., R. Farneti (2023)](https://doi.org/10.3389/fmars.2023.1208052); [Narayanasetti et al. (2022)](https://doi.org/10.1007/s00382-022-06224-1); [Todd et al. (2020)](https://doi.org/10.1029/2019MS002027))

### Co-ordinated Ocean-Ice Reference Experiments ([CORE](https://www.clivar.org/omdp/core))
___
Ocean-ice model experiments are useful since they are less costly than fully coupled experiments, they can be used in hindcast mode to reproduce the history of ocean and ice variables and hence help in the interpretation of observations, they allow for the understanding of processes in the absence of biases introduced by the atmospheric model and hence potentially give superior representations (compared to the ocean component of a coupled model) of key physical, chemical and biological processes and so help in model development.

Both CORE-I and CORE-II simulations provide a framework to evaluate ocean model performance, to study mechanisms of ocean phenomena and their variability from seasonal to decadal timescales, to identify forced variability changes, and to develop mechanistic descriptions of observed climate variability and change.

([Rahaman et al. (2020)](); [Tseng et al. (2016)](); [Danabasoglu et al. (2016)](); [Farneti et al. (2015)](); [Downes et al. (2015)](); [Sitz et al. (2015)](); [Griffies et al. (2014)](); [Danabasoglu et al. (2014)]())

### JRA-55 based surface dataset for driving ocean-sea ice models ([JRA55-do](https://climate.mri-jma.go.jp/pub/ocean/JRA55-do/index.html))
___
JRA55-do (Tsujino et al., 2018) is a surface dataset for driving ocean-sea ice models and used in phase 2 of OMIP (OMIP-2).

I have written some notes on how to use JRA55-do in MOM5 [here](https://mom-ocean.github.io/assets/pdfs/MOM5_JRA55do.pdf).

### An Intermediate Complexity ocean-atmosphere-land-ice Coupled Model (ICCMv1.0)
___
An idealized coupled ocean-atmosphere-land-ice model was developed to study climate variability at interannual to interdecadal and longer time scales and to identify mechanisms of ocean-atmosphere interactions.

The model uses the three-dimensional primitive equations for both ocean and atmosphere, but is simplified from a ‘state of the art’ model in two respects: the model uses simplified physics and parameterization schemes, especially in the atmosphere, and the geometry and geography are much simplified. These simplifications provide considerable savings in computational expense and, perhaps more importantly, allow mechanisms to be investigated more cleanly and thoroughly than with a more elaborated model. For example, the model allows integrations of several millennia as well as broad parameter studies.

For the ocean, the model uses the free surface primitive equations Modular Ocean Model (MOM) in its 4p0 version. The FMS sea-ice model SIS is coupled to the oceanic grid in its standard configuration. The atmospheric component is made of the FMS B-grid moist primitive equation atmospheric dynamical core with highly simplified physical parameterisations (Frierson, 2005). A simple bucket model is implemented for our idealised land following the FMS Land model.

The coupled model is a simplified version of the Geophysical Fluid Dynamics Laboratory (GFDL) CM2.0 and two (geometrical) versions are implemented: an Atlantic-like and an Aquaworld configuration.
In the first case our ocean component is that of a single ocean basin (Atlantic) with an Antarctic Circumpolar Current simulated by cyclic open boundary conditions. Perhaps the most striking simplification of our model's Atlantic configuration is in its geometry; in fact, we decided to focus on basin-scale ocean-atmosphere interactions and therefore opted for a sector model, in which the ocean is represented by a single basin and the atmosphere above it is a 120$`^o`$ sector. This has some similarities with the QG framework proposed in Hogg et al (2003b) and Kravtsov et al (1005), and approaches the modelling strategy of Saravanan at al (1995, 1997), where a 2-D zonally averaged ocean sector model is used together with a dynamical idealized atmosphere.
Several experiments were performed with this configuration in which the geometry (no Drake Passage, wider ocean basin, shallower ocean basin) or a parameter/parameterization was altered (laplacian horizontal diffusivity scheme for tracers, vertical diapycnal diffusivity, horizontal resolution, etc.).
The second configuration, Aquaworld, is that of a 360$`^o`$ atmosphere overlying a dynamic ocean. No continents are present, though in one experiment a few ridges constraint the circulation in the ocean. This set-up resembles the models presented in Smith at al (2006) and Marshall at al (2007).
Both configurations incorporate the eddy parameterization of Gent-McWilliams, which is believed to improve convection in coarse-resolution ocean models and a constant value is used for the vertical diffusivity in the ocean, Kv, in order to clearly explore dependencies on this parameter.
Idealized initial temperature and salinity conditions are applied to the ocean at rest and the sea-ice model is coupled to the ocean. 
The moist primitive equations atmospheric component employs simplified parameterizations of atmospheric processes following Frierson (2005). These changes imply a considerable computational gain, retaining a good representation of the atmospheric climate at both tropical and extra-tropical latitudes (Frierson at al, 2006).
Finally, the land model is reduced to a single bucket land, with constant water availability and heat capacity, and a simple redistribution of precipitated water back into the ocean.

The model components and new parameterizations retain the original modularity, in order to allow the coupled model to recover complexity in any of its parts.
It should be emphasized at this point that the objectives of this modelling initiative are not those of reproducing an accurate climate in all its details, but rather to test some mechanisms in the coupled ocean-atmosphere system and trying to understand the relative role of its different components. A more realistic response could be achieved in both the ocean and atmosphere, but with a computational cost and with increasing complexity in the model's physics, which would be counterproductive to our initial objective.

The model has been used for several fundamental studies on the coupled ocean-atmosphere system:

* [Farneti, R. and G. K. Vallis (2013), Meridional energy transport in the coupled atmosphere-ocean system: Compensation and partitioning. **J of Climate**, 26, 18, 7151-7166.]()
* [Farneti, R. and G.K. Vallis (2011), Mechanisms of interdecadal climate variability and the role of ocean-atmosphere coupling. **Climate Dynamics**,  36, 1, 289--308.]()
* [Vallis, G. K. and R. Farneti (2009), Meridional energy transport in the coupled atmosphere-ocean system: Scaling and numerical experiments, **QJRMS**, 135, 644, 1643-1660]()
* [Farneti, R. and G.K. Vallis (2009), An Intermediate Complexity Climate Model (ICCMp1) based on the GFDL Flexible Modelling System, **GMD**, 2, 1, 73-88]()

