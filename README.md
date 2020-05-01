# Analytical solution to runoff on hillslopes with curvature: numerical and laboratory verification: supplementary data and code

Dana Lapides [1], Cy David [1], Anneliese Sytsma [2], David Dralle [3], and Sally Thompson [4,5]

[1] Department of Earth and Planetary Science, University of California, Berkeley

[2] Department of Environmental Design, University of California, Berkeley

[3] Department of Geology, Sacramento State University

[4] Department of Civil and Environmental Engineering, University of California, Berkeley

[5] Department of Environmental Engineering, University of Western Australia

[![DOI](https://zenodo.org/badge/180637473.svg)](https://zenodo.org/badge/latestdoi/180637473)


This repository includes programs to run the solution to the Hillslope Storage Kinematic Wave Equation for Overland Flow, results from ParFlow (1,2,3,5) simulations described by (4) with a program to visualize the data, and results from laboratory experiments described by (4) with a program demonstrating data smoothing methods and another program showing the hydrograph parameterization for comparison between analytical and laboratory methods. A file tree of included content is below:

* Hillslope_Storage_Analytic_symbols_table.pdf
* Hillslope_storage_KW_analytic.ipynb
* Hillslope_storage_KW_numerical.ipynb
* Experiment_data
  * raw_data.xlsx
  * Hillslope_Smoothing.ipynb
  * smooth_hydrograph_data.csv
  * Experimental_analysis.ipynb
* ParFlow
  * ParFlow_Visualization.ipynb
  * Boundary_flow_data
  * Flow_depth
  * Hydrograph_data

Hillslope_Storage_Analytic_symbols_table.pdf includes a table of symbols used in the code and README files for this project.

The jupyter notebook titled: Hillslope_storage_KW_analytic includes the solution to the hillslope-storage kinematic wave equation for overland flow for a width function described by an exponential of the form w=ce^(ax), where w is the contour width, i.e. distance between limiting streamlines, x is the distance downhill from the divide, a is a constant describing hillslope convergence/divergence, and c is a constant describing the size of the hillslope in the cross-slope direction. The jupyter notebook runs this solution for user-defined values of a, c, rainfall rate r, storm length tr, infiltration rate f, roughness parameter alpha, and hillslope length (xend-xtop, where xend is the outlet location and xtop is the divide location). This solution is valid for m=2 only. The notebook produces characteristic nets for the storms as well as hydrographs of q or Q, depending on user preference. The program also prints the value of tc and qmax for each run.

The jupyter notebook titled: Hillslope_storage_KW_numerical includes the solution to the hillslope-storage kinematic wave equation for overland flow for a width function described by an exponential of the form w=ce^(ax), where w is the contour width, i.e. distance between limiting streamlines, x is the distance downhill from the divide, a is a constant describing hillslope convergence/divergence, and c is a constant describing the size of the hillslope in the cross-slope direction. The jupyter notebook runs this solution for user-defined values of a, c, rainfall rate r, storm length tr roughness parameter alpha, and hillslope length (xend-xtop, where xend is the outlet location and xtop is the divide location). This solution is valid for any user-defined value of m but only for zero infiltration f=0. The notebook produces characteristic nets for the storms as well as hydrographs of q or Q, depending on user preference. The program also prints the value of tc and qmax for each run.

The directory Experiment_data includes an excel file with the raw data (raw_data.xlsx), a program that explores different data smoothing methods (Hillslope_Smoothing.ipynb), a csv of smooth data (smooth_hydrograph_data.csv), and a program that compares analytical hydrographs to experimental results (Experimental_Analysis.ipynb), as described in (4).

The directory ParFlow includes data for all of the ParFlow simulations referred to in (4) (including flow hydrographs in Hydrograph_data, flow data across the boundary in the Boundary_flow_data directory, and flow depth across the boundary in the Flow_depth directory) and a program to visualize the data. The reported data are for an exponential width hillslope. The columns in the data text files are as follows: (0) Timestep number with timesteps in increments of 1 minute, (1) total flow out the bottom boundary during that timestep (m3/s), (2) standard deviation of flow values at eat cell along the bottom boundary (m3/s), (3) mean flow value along the bottom boundary (m3/s). The included jupyter notebook titled: ParFlow_Visualization.ipynb.

For beginners to Python and jupyter notebook:

In each of the two jupyter notebook simulations, the code is broken down into 4 different blocks. The first block includes module dependencies, which you must install before running the notebook in addition to jupyter notebook. The second block contains the equations described by Lapides et al. n.d.. The third block solves for characteristic nets and hydrograph data and plots the characteristic nets. This block includes a number of different options that users can change, commented in the code. The final block plots a hydrograph of q or Q depending on user preference. User-defined parameters are marked at the top of the block. 

To run the code, run each block sequentially. If you make changes to user preferences, you need to rerun only the block where you made changes and any subsequent blocks. Prior blocks should be unaffected.




References
[1] Jones, J.E. and Woodward, C.S. (2001). Newton–Krylov-multigrid solvers for large-scale, highly heterogeneous, variably saturated flow problems. Advances in Water Resources, 24(7), 763–774, doi:10.1016/S0309-1708(00)00075-0.

[2] Ashby S.F. and Falgout, R.D. (1996). A Parallel Multigrid Preconditioned Conjugate Gradient Algorithm for Groundwater Flow Simulations. Nuclear Science and Engineering, 124(1), 145-159.

[3] Kollet, S.J. and Maxwell, R.M. (2006). Integrated surface-groundwater flow modeling: a free-surface overland flow boundary condition in a parallel groundwater flow model. Advances in Water Resources, 29(7), 945-958, doi:10.1016/j.advwatres.2005.08.006.

[4] CITATION FOR MY PAPER

[5] Maxwell, R.M. (2013) A terrain-following grid transform and preconditioner for parallel, large-scale, integrated hydrologic modeling. Advances in Water Resources, 53, 109-117, doi:10.1016/j.advwatres.2012.10.001.


