This directory contains the raw data plotted in Fig. 1 and Fig. S1.

Files named 'coex-*.dat' contain coexistence points computed from thermodynamic integration or direct coexistence, as indicated. These correspond to the blue line, the brown line and the red triangles in the figure.

The 'discontinuity-kink.dat' file contains approximate points where there is a discontinuity in the density and enthalpy in brute-force simulations. This corresponds to the cyan dashed line in the figure.

The files in the 'panel-b' subdirectory give displacement data plotted in panel b. The first column is an index; the second column gives the distance in angstrom, the third column gives a scaled distance (relative to the overall simulation box size), and the fourth column gives the relative frequency of proton displacement after 0.4 s of MD simulations. In the plots shown in Fig. 1(b), we plotted column 2 on the x axis and column 4 on the y axis (on a log scale).

The directory 'chemical-potentials' contains data plotted in Fig. 1(c) and (d), as indicated in the column headers.

The directories 'isobars' and 'isotherms' contain the underlying raw data used in thermodynamic integration, as indicated in the column headers. Several of these are plotted in Fig. S1.


Finally, in order to generate all these data, the files input-isobar.lammps and input-isotherm.lammps give example Lammps scripts for isobar and isotherm generation. The scripts compute the appropriate quantities needed for thermodynamic integration, and also the displacement statistics used to generate Fig. 1(b).
In order to run these simulations, the 'RUNNERDIR' string should be updated to give the directory in which the machine-learning potential parameterisation is located (i.e. the files input.nn, scaling.data, weights.001.dat, weights.008.data). These can be obtained from https://github.com/BingqingCheng/superionic-water/tree/main/nnp or the 'Supplementary Data 1' archive available at https://doi.org/10.1038/s41567-021-01334-9
