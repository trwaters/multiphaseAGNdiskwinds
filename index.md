## Simulations
The animations below are solutions to the equations of non-adiabatic gas dynamics, 
obtained with [Athena++](https://github.com/PrincetonUniversity/athena-public-version/wiki) (v19).  
These are axisymmetric (2.5D) calculations performed in spherical coordinates.  
For further details on the numerics, see the appendix of the paper.  

### Mid-res runs
Here we show an animated version of Fig. 6, zooming into the region within 100 R_IC to 
show the formation of irradiated atmospheric fragments (IAFs).  These are the characteristic
structures formed by thermal instability operating within a vortex in the upper atmosphere 
located just below the thin transition layer separating the atmosphere and disk wind.  
These runs have an effective resolution of roughly dx = 0.3 R_IC = 10^4 R_s (with R_s = 2GM/c^2 the Schwarzschild radius),
so IAFs (which evolve into 'tsunami-like' features) are fluid phenomena occuring on enormous size scales.  


### Hi-res runs
Our hi-res run has an extra level of statish mesh refinement, so dx is about 400 R_s.

### Acknowledgements
These simulations were run on the Institutional Computing clusters at Los Alamos National Laboratory under allocation award w19_rhdccasims (PI: T. Waters).  We thank the [high performance computing team](https://www.lanl.gov/org/ddste/aldsc/hpc/index.php) for their continued efforts, as well as the developers of the public GRMHD code [Athena++](https://github.com/PrincetonUniversity/athena-public-version/graphs/contributors). 
