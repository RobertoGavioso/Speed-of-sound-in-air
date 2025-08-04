The present GitHub project was created to make available, for public use, 
Labview executable and source files needed to calculate speed of sound in humid air
as a function of the main parameters of influence, namely temperature T, pressure p, relative humidity hr, 
carbon dioxide concentration xCO2 and acoustic frequency f. 
The validity of the model extends over the temperature range, 200 K < T < 647 K, for pressures up to 10 MPa,
for arbitrary relative humidity (from dry air up to saturation), and arbitrary CO2 content and acoustic frequency.  

Further details about the model and its uncertainty are available in the paper:

Speed of sound in humid air: accurate thermodynamic model and experimental validation 
R. M. Gavioso, M. Astrua, M. Zucco, M. Pisani 

submitted for publication in J. Phys. Chem. Ref. Data in August 2025.

The Labview files in the GitHub project are organized in two main directories, namely:

1) "executable labview files"
____________________________

Which contains the following three executables:

SoS_AIR_2025.exe, which outputs speed of sound in humid air and its standard uncertainty given the input parameters T, p, xw, xCO2, f;
Plot & Save SoS.exe, allows to create plots, and save in tabular form text files listing speed of sound in humid air and its standard uncertainty 
given an arbitrary choice to fix at constant value two out of four of the input parameters T, p, xw, f and to let one of the remaining parameters to vary, 
with arbitrary resolution, between limiting bounds.
T from SoS_AIR_2025.exe, Given a value of experimentally measured speed of sound in air in input, for a specified set of parameters (p, xw, xCO2, f) 
this software allows to calculate the corresponding acoustic temperature T by iteration, using a simple bisection method. 

To run on a computer where Labview software is not installed, these executables
require prior installation of the freeware LabVIEW Runtime for Labview 2016 (32 bit)
which can be downloaded at the following link:

	https://www.ni.com/en/support/downloads/software-products/download.labview-runtime.html?srsltid=AfmBOoqbvFkfD0_r786NzkpCeRT8KszK-H0zPMm1fq7oQjzkC5q5hG18#310816

2) "source labview files"
___________________________

which contains three main source (vis), namely: "SoS_AIR_2025_v1_0_2025.vi"; "Plot & Save SoS_AIR_v1_0_2025.vi";
"T from SoS_AIR_v1_0_2025.vi" corresponding to the three executables commented above, 
and in additiona a total of 41 subvis, which are required by the main source files.

All these source files can be run, debugged and modified by any user with an installed Labview version later than version 2016 (64 bit).
It is suggested that the total 44 files wuold be downloaded and copied in the same directory.  

	

