# FEM_BEM_EXAMPLES
Problems related to Finite Element Method (FEM) and Boundary Element Method (BEM) specifically related to modelling transducers (CMUT) for underwater acoustics application using bempp_cl,fenicsx and gmsh

# FILES IN THIS REPOSITORY

## 1. 1_way_coupling.ipynb:
One way FEM-BEM coupling to model CMUT for underwater acoustics application. Solved linear elasticity equation in FEM and calculated displacement. Using displacement     calculated normal velocity on the vibrating surface. Solved Helmholtz equation in BEM for infinite domain. File uses cube.msh

## 2. 2_way_coupling.ipynb:
Two way FEM-BEM coupling using blocked operators to model CMUT for underwater acoustics application. Solved linear elasticity equation in FEM and Helmholtz equation in BEM for infinite domain. Pressure calculated through BEM opposes the displacement. File uses cube.msh. Displacement visualized in paraview: displacement_2_way_coupling.pmg

## 3. actual_bem.ipynb:
Replicated official bempp tutorial but for water as medium and a specific surface mesh (mesh_trial.msh).

## 4. loudspeaker_axis_symmetry.ipynb:
Replicated louspeaker problem for an axis symmetric geometry: cone2.msh

## 5. scattering_2D.ipynb:
Scattering from a 2D geometry, circle. Since bempp_cl does not enables solving for 2D BEM equations directly, here a cylinder with negligible height is taken as a circle. Uses cylinder2.msh
