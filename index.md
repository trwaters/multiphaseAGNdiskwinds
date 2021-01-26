## Animations
The animations below are of time-dependent solutions to the equations of non-adiabatic gas dynamics described in this [submitted paper](https://arxiv.org/abs/2101.09273), designed to model the parsec-scale environments of AGN accretion disks that are being subjected to irradiation by ionizing X-ray photons (assumed to be produced in a hot corona in the immediate vicinity of the supermassive black hole).  These are axisymmetric (2.5D) calculations performed in spherical coordinates using [Athena++](https://github.com/PrincetonUniversity/athena-public-version/wiki) (v19).  For further details on the numerics, see the appendix of the paper.  

### Mid-res runs
Here is a movie of the initial evolution starting from constant pressure initial conditions.  This shows the 'construction' of the full thermal wind solution consistent with the imposed boundary conditions.  The final state -- a disk atmosphere and a tenuous disk wind -- is insensitive to the initial conditions.  In all of the runs below, time is shown in units of the Keplerian orbital period at 1 R_IC.  The red contour marks where the Bernoulli function vanishes, indicative of a transition from bound to unbound flow.  
<video poster="midres_nICs.png" width="675" height="750" controls preload> 
    <source src="midres_n-early.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="midres_n-early.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

Next we show an animated version of Fig. 6 that zooms into the region within 100 R_IC where irradiated atmospheric fragments (IAFs) first form.  IAFs are the characteristic structures resulting after a hot bubble buoyantly rises and disrupts the thin transition layer separating the atmosphere and disk wind.  This bubble in turn forms as a consequence of thermal instability (TI) operating within a vortex in the upper atmosphere located just below the transition layer.  These runs have an effective resolution of roughly dx = 0.3 R_IC = 10^4 R_s (with R_s = 2GM/c^2 the Schwarzschild radius), so IAFs (which evolve into 'tsunami-like' features spanning ~10 R_IC) are fluid phenomena occuring on enormous size scales relative to the supermassive black hole itself.  

<video poster="midres_npreview.png" width="675" height="750" controls preload> 
    <source src="midres_n-zoom.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="midres_n-zoom.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

Starting around t=1200, the brown gas engulfed within the crest of the IAF can be seen becoming a more whitish color, indicating that the gas is becoming more rarefied due to a rise in temperature.  TI is continuously operating within this gas, hence continuous heating is taking place.  This can also be seen happening within the bubbles underneath the IAFs.

Here is an animated version of Fig. 9 showing the full domain.  Starting from t=1200, we evolve for 1.6 orbits at r_out, long enough to reach a fully developed clumpy wind solution.  For NGC 5548, the system we used to derive characteristic heating and cooling rates, this corresponds to 6 Myr of evolution.  
<video poster="midres_nfull-preview.png" width="675" height="750" controls preload> 
    <source src="midres_nfull.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="midres_nfull.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

### Hi-res runs
Below is an animated version of Fig. 8, showing our hi-res run that has an extra level of static mesh refinement (so dx is about half as small). This increase in resolution is sufficient to resolve the [vortex shedding](https://en.wikipedia.org/wiki/Vortex_shedding) process that accompanies the appearance of IAFs.  Akin to uniform flow past a cylinder, IAFs are obstructions to the smooth disk wind.  
<video poster="midres_npreview.png" width="675" height="750" controls preload> 
    <source src="hires_nzoom.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="hires_nzoom.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

Finally, here is an animated version of the snapshots in Fig. 11, showing maps of the ionization structure rather than the number density.
<video poster="hires_xipreview.png" width="675" height="750" controls preload> 
    <source src="hires_xi.mp4" media="only screen and (min-device-width: 568px)"></source> 
    <source src="hires_xi.mp4" media="only screen and (max-device-width: 568px)"></source> 
</video>

For this run, we also computed synthetic X-ray line profiles along two lines of sight through the multiphase region and found that the K-alpha lines of Fe XXV and Fe XXVI can feature multiple absorption troughs.  Strong X-ray lines such as O VIII Ly-alpha show a more gradual desaturation compared to smooth stages of evolution.  For details on this, please refer to our discussion section and Fig. 14. 
![synthetic line profiles](webpageLPs.png "from Fig 14")

### Acknowledgements
These simulations were run on the Institutional Computing clusters at Los Alamos National Laboratory under allocation award w19_rhdccasims (PI: T. Waters).  We thank the [high performance computing team](https://www.lanl.gov/org/ddste/aldsc/hpc/index.php) for maintaining this system for open science use.  We also thank the [Athena++](https://github.com/PrincetonUniversity/athena-public-version/graphs/contributors) developers for their continued efforts. 
