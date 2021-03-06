simutil
=======

Scripts and small utilitary programs to assist in simulations (using DL_POLY, GROMACS or Towhee). The utilitaries are based on a specific program's output or input files. The tools are used to aid in the research carried out at Instituto Superior Técnico (IST), Universidade de Lisboa, Portugal.

Every tool is designed to work with as little input as possible. Idealy the programs run without the need to provide any input, the tool runs taking what it need from the folder in which it is called.

## Folder structure
The folder names are self explanatory. None the less it might be useful to lay out the reasoning behind it.

* ```bin``` - In the bin folder you will find compiled programs.
* ```source``` - In the source folder live the .f90 files with the respective code for each tool. 
* ```test``` - Finaly, in the test folder exists a folder with the necessary files to run the compiled code as a test, as well as the supposed output for that test.

##Utilities
The utilities uncompiled, FORTRAN 90, files are located in the ```source``` folder. A compiled version is found in the ```bin``` folder. As with the folder structure, the utilities are named in such a way to make it easy to grasp their functionality.

* ```cfg2pdb``` - Convert a CONFIG file, from DL_POLY, into a PDB (Protein Data Bank) file to be used in RASMOL. (The output can, of course, be used elsewhere.)
* ```gro2cfg``` - Convert a GROMACS ```.gro``` file into a DL_POLY CONFIG file.
* ```surfangle``` - Determine the angle between molecules forming a monolayer on top of water, and the surface of the water. Can be easely fitted for other systems. (Uses the DL_POLY HISTORY file.)
* ```surfplane``` - Determine the cluster of molecules that corresponde to the top surface in a simulation to obtain surface interactions/properties. (Uses the DL_POLY HISTORY file.)