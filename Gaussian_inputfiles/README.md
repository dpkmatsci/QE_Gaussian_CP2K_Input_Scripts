
## Documentation

The above folders contain the input script for Quantum Chemistry calculations in Gaussian16. Useful links : [https://www.youtube.com/@GaussianInc], [https://www.youtube.com/playlist?list=PLHB5VxMFpHNP6Arppjxb72Lq0Ym1xWkof]

Input and output files are in *.gjf and *.OUT format respectively.

Geometry optimization:
```
Input files for geometry optimization of calcium silicate dimer with exchange correlation WB97XD with water as solvent.
```

TS_Optimization: 
```
Input files for the calculation of transition state using different methods available in Gaussian16. 
dimersiohts.gjf : Prediction of transition state for breaking of Si-OH bond in silicate dimer using Berny optimization method (TS Berny). In this case input geometry must be very close to actual transition state otherwise it will lead to error. Here force constant needs to be calculated which can be done only initially (opt = (calcfc,ts)) or at each optimization step (opt=(calcall, ts))

c2sdimersiohts.gjf : Calculation of transition state for breaking of Si-OH bond in silicate dimer using QST2 method. In this method, molecular geometry from both reactant and product state needs to be provided. However, this input is not exact reactant and product but two geometries very close to transition state but lying on the side of reactant and prodcut.

c2sdimertsnw.gjf : Calculation of transition state for the formation of Si-O bond in silicate dimer using QST3 method. Here input is three molecular geometries one from each reactant and product side alongwith possible transition state geometry. 
```

NBO_calculation: 
```
Codes for calculation of NBO charge in optimized geometry of calcium silicate dimer. The default scheme implemented in Gaussian16 is NBO version 3. Latest available version is NBO7.0 which needs to be incorporated separately.
``` 

IRC_calculation: 
```
Codes for Intrinsic reaction coordinate (IRC) calculation for two different transition state geometries. 
```

PES_Scan: 
```
Input files for the scanning of potential energy surface (PES) across a particular internl coordinate. The output file for dimersiohscn is incomplete but results can be viewd in Gaussview. Another example pf5scn demonstrates the change of potential energy during pseudorotation in PF5.
PES scanning is very useful in locating transition states or achieving a geometry quite close to the transition state. First select one or two possible reaction coordinate. Perform the PES scanning along these and identify the geometries lying close to the peak. Along with energy check the RMS gradient curve also. The transition states have almost zero RMS energy gradient norm.  
```

