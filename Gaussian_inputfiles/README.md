
## Documentation

The above folders contain the input script for Quantum Chemistry calculations in Gaussian16. Useful links : [https://www.youtube.com/@GaussianInc], [https://www.youtube.com/playlist?list=PLHB5VxMFpHNP6Arppjxb72Lq0Ym1xWkof]

Input and output files are in *.gjf and *.OUT format, respectively.

Geometry optimization:
```
Input files for geometry optimization of calcium silicate dimer with exchange correlation WB97XD with water as solvent.
```

TS_Optimization: 
```
Input files for the calculation of the transition state using different methods available in Gaussian16. 
dimersiohts.gjf: Prediction of transition state for breaking of Si-OH bond in silicate dimer using Berny optimization method (TS Berny). In this case, the input geometry must be very close to the actual transition state; otherwise, it will lead to an error. Here force constant needs to be calculated, which can be done only initially (opt = (calcfc,ts)) or at each optimization step (opt=(calcall, ts))

c2sdimersiohts.gjf: Calculation of transition state for breaking of Si-OH bond in silicate dimer using QST2 method. In this method, the molecular geometry from both the reactant and product states needs to be provided. However, this input is not the exact reactant and product but two geometries very close to the transition state, but lying on the side of the reactant and product.

c2sdimertsnw.gjf: Calculation of transition state for the formation of Si-O bond in silicate dimer using QST3 method. Here input is three molecular geometries, one from each reactant and product side along with the possible transition state geometry. 
```

NBO_calculation: 
```
Codes for the calculation of the NBO charge in the optimized geometry of calcium silicate dimer. The default scheme implemented in Gaussian16 is NBO version 3. The latest available version is NBO7.0, which needs to be incorporated separately.
``` 

IRC_calculation: 
```
Codes for Intrinsic reaction coordinate (IRC) calculation for two different transition state geometries. 
```

PES_Scan: 
```
Input files for the scanning of the potential energy surface (PES) across a particular internal coordinate. The output file for dimersiohscn is incomplete, but results can be viewed in Gaussview. Another example pf5scn demonstrates the change of potential energy during pseudorotation in PF5.
PES scanning is very useful in locating transition states or achieving a geometry quite close to the transition state. First select one or two possible reaction coordinates. Perform the PES scanning along these and identify the geometries lying close to the peak. Along with energy, check the RMS gradient curve. The transition states have almost zero RMS energy gradient norm.  
```

