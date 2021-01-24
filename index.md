## Animations
The animations below are of time-dependent solutions to the equations of non-adiabatic gas dynamics described in this [submitted paper](https://arxiv.org/), designed to model the parsec-scale environments of AGN accretion disks that are being subjected to irradiation by ionizing X-ray photons (assumed to be produced in a hot corona in the immediate vicinity of the supermassive black hole).  These are axisymmetric (2.5D) calculations performed in spherical coordinates using [Athena++](https://github.com/PrincetonUniversity/athena-public-version/wiki) (v19).  For further details on the numerics, see the appendix of the paper.  

### Mid-res runs
Here we show an animated version of Fig. 6 that zooms into the region within 100 R_IC where irradiated atmospheric fragments (IAFs) first form.  IAFs are the characteristic structures resulting after a hot bubble buoyantly rises and disrupts the thin transition layer separating the atmosphere and disk wind.  This bubble in turn formed as a consequence of thermal instability operating within a vortex in the upper atmosphere located just below the transition layer.  These runs have an effective resolution of roughly dx = 0.3 R_IC = 10^4 R_s (with R_s = 2GM/c^2 the Schwarzschild radius), so IAFs (which evolve into 'tsunami-like' features spanning ~10 R_IC) are fluid phenomena occuring on enormous size scales relative to the supermassive black hole itself.  

<video poster="midres_npreview.png" width="675" height="750" controls preload> 
    <source src="midres_n-zoom.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="midres_n-zoom.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

### Hi-res runs
Below is an animated version of Fig. 8, showing our hi-res run that has an extra level of statish mesh refinement (so dx is about half as small).  
This increase in resolution is sufficient to resolve the [vortex shedding](https://en.wikipedia.org/wiki/Vortex_shedding) process that accompanies the appearance of IAFs.  

Finally, here is an animated version of the snapshots from in Fig. 11, showing maps of the ionization structure rather than the number density.
<video poster="hires_xipreview.png" width="675" height="750" controls preload> 
    <source src="hires_xi.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="hires_xi.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>


### Acknowledgements
These simulations were run on the Institutional Computing clusters at Los Alamos National Laboratory under allocation award w19_rhdccasims (PI: T. Waters).  We thank the [high performance computing team](https://www.lanl.gov/org/ddste/aldsc/hpc/index.php) for maintaining this system for open science use.  We also thank the [Athena++](https://github.com/PrincetonUniversity/athena-public-version/graphs/contributors) developers for their continued efforts. 
