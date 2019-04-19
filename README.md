# Hillslope Storage Kinematic Wave
This repository includes programs to run the solution to the Hillslope Storage Kinematic Wave Equation for Overland Flow and results from ParFlow (1,2,3,5) simulations described by (4). 

The jupyter notebook titled: Hillslope_storage_KW_analytic includes the solution to the hillslope-storage kinematic wave equation for overland flow for a width function described by an exponential of the form w=ce^(ax), where w is the contour width, i.e. distance between limiting streamlines, x is the distance downhill from the divide, a is a constant describing hillslope convergence/divergence, and c is a constant describing the size of the hillslope in the cross-slope direction. The jupyter notebook runs this solution for user-defined values of a, c, rainfall rate r, storm length tr, infiltration rate f, roughness parameter alpha, and hillslope length (xend-xtop, where xend is the outlet location and xtop is the divide location). The notebook produces characteristic nets for the storms as well as hydrographs of q or Q, depending on user preference. The program also prints the value of tc and qmax for each run.

A table of variables used in the code is included in this repository as well.

For beginners to Python and jupyter notebook:

The code is broken down into 4 different blocks. The first block includes module dependencies, which you must install before running the notebook in addition to jupyter notebook. The second block contains the equations described by Lapides et al. n.d.. The third block solves for characteristic nets and hydrograph data and plots the characteristic nets. This block includes a number of different options that users can change, commented in the code. The final block plots a hydrograph of q or Q depending on user preference. User-defined parameters are marked at the top of the block. 

To run the code, run each block sequentially. If you make changes to user preferences, you need to rerun only the block where you made changes and any subsequent blocks. Prior blocks should be unaffected.

The folder ParFlow_hydrographs includes hydrograph data for all of the ParFlow simulations referred to in (4). The reported data are for an exponential width hillslope. The columns are as follows: (0) Timestep number with timesteps in increments of 1 minute, (1) total flow out the bottom boundary during that timestep (mm3/hr), (2) standard deviation of flow values at eat cell along the bottom boundary (mm3/hr), (3) mean flow value along the bottom boundary (mm3/hr).


References
[1] Jones, J.E. and Woodward, C.S. (2001). Newton–Krylov-multigrid solvers for large-scale, highly heterogeneous, variably saturated flow problems. Advances in Water Resources, 24(7), 763–774, doi:10.1016/S0309-1708(00)00075-0.

[2] Ashby S.F. and Falgout, R.D. (1996). A Parallel Multigrid Preconditioned Conjugate Gradient Algorithm for Groundwater Flow Simulations. Nuclear Science and Engineering, 124(1), 145-159.

[3] Kollet, S.J. and Maxwell, R.M. (2006). Integrated surface-groundwater flow modeling: a free-surface overland flow boundary condition in a parallel groundwater flow model. Advances in Water Resources, 29(7), 945-958, doi:10.1016/j.advwatres.2005.08.006.

[4] CITATION FOR MY PAPER

[5] Maxwell, R.M. (2013) A terrain-following grid transform and preconditioner for parallel, large-scale, integrated hydrologic modeling. Advances in Water Resources, 53, 109-117, doi:10.1016/j.advwatres.2012.10.001.


