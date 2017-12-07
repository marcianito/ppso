Particle Swarm Optimization and Dynamically Dimensioned Search, optionally using parallel computing based on Rmpi
======================================================================

# This is a fork of ppso (version 0.9994) from https://www.rforge.net/ppso/ #

Originally written and maintained by Till Franke.

## Description
(Optionally parallelized) optimization using PSO (Particle Swarm Optimzation) or DDS (Dynamically Dimensioned Search) algorithms, which excell for multidimensional (multi-parameter) functions with many local extrema and a restricted number of function evaluations.
The parallelized version builds on Rmpi and is intended for highly computationally intensive objective functions (>20 s evaluation time).
Another focus of this package is the possibility to resume interrupted optimization runs from the intermediate project files.
These features make this package useful for the automatic calibration of complex numerical models (e.g. hydrological models). 

For bug fixes, comments or further development please open an issue or contact: franke@uni-potsdam.de or mreich@posteo.de.

## Installation

1. Start R
2. Install package via devtools: 
`devtools::install_github("marcianito/ppso")`

3. load packages: 
`library(ppso)`;

## Dependencies

### Computationally
* r-base version 3.3.1
* following R-packages: devtools,  ??
* system libraries for devtools

in debian install using: 
`apt-get update && apt-get install libssl-dev`

<!-- ### Data-wise -->
<!-- It is necessary to have a time series of observed gravity data (could be synthetic). -->
<!--  -->
<!-- ## Processing -->
<!--  -->
<!-- 1. Start R -->
<!-- 2. Load infiltration_example.r script -->
<!-- 3. Modify according to description below -->
<!-- 4. Run script and look at outputted results -->
<!--  -->
<!-- ## Infiltration modeling procedure (computations) -->
<!-- #### For more details, please look at the vignette or the corresponding help-files (within R). -->
<!--  -->
<!-- All changes should be done in a new file following (or a copy of) the reduction_example.r file. -->
<!--  -->
<!-- (Step 2 is only explanatory for what the script does; no modifications necessary.) -->
<!--  -->
<!-- 1. Setup:  -->
<!--     * _Directory and configs (input / output, file extentions, enable plotting)_ -->
<!--     * _Gravimeter coordinates (x, y, z + height of sensor)_ -->
<!--     * _Model domain (x and y extensions)_ -->
<!--     * _Discretization and vertical model extent_ -->
<!--     * __ -->
<!--     * _Set correct file to load for DEM input_ -->
<!--     * _Input file settings (data dimensions, order of data columns from input files)_ -->
<!--     * _Input file names (DEM, observed gravity signal, .. etc !?)_ -->
<!-- 2. Calculations:  -->
<!--     * _Construct surface grid_ -->
<!--     * _Create gravity component grid_ -->
<!--     * __ -->
<!--     * _Plot all time series_ -->
<!-- 5. Run the entire script and look at output files -->
<!--  -->
