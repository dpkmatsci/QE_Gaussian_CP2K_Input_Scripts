\## Documentation



The input scripts for cell relaxation, slab relaxation and ab-initio molecular dynamics (AIMD) in open source package CP2K have been provided in above folders.
Useful links for CP2K: [https://www.cp2k.org/], [https://manual.cp2k.org/trunk/], [https://www.cp2k.org/exercises]

Input and output files are in \*.inp and \*.out format.



Small cell relaxation for Alumina

```bash

&nbsp;     Input script without dispersion correction and with different dispersion schemes.

&nbsp;     File with atomic coordinates in initial unrelaxed state: alumina\_unrlxd.xyz

```



Slab relaxation and AIMD for Silica systems

```bash

&nbsp;     Initial unrelaxed file in Silica slab relaxation: silica\_zslabepoxyoptdft.xyz   

&nbsp;     Initial unrelaxed file in Silica-water slab relaxation: silica\_zslabepoxywtrini.xyz

&nbsp;     Initial Atomic coordinates for AIMD simulation: silica\_zslabepoxywtroptdft\_rlxd.xyz

&nbsp;     Summary of convergence parameters at different optimization steps in relaxation: geom\_opt-1\_0.geoLog  

```

