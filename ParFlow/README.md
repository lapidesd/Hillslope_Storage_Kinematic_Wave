
This folder includes folders containing results from numerical simulations with ParFlow (1,2,3,5) on divergent/convergent hillslopes with exponential width functions (w = ce^(ax) ) as described by (4). The values of a range from -0.1 to 0.1. This folder also includes a program to visualize the data titled parflow_visualization.ipynb.

The jupyter notebook titled Parflow_Visualization.ipynb includes blocks that visualize each type of data provided including: hydrograph data, boundary flow data, and boundary depth data. Additional blocks show the differences between simulations run at different resolutions.

The folder Hydrograph_data includes hydrograph data for all of the ParFlow simulations referred to in (4), Flow_depth includes the flow data along the boundary at the time of equilibrium peak flow, and Boundary_flow_data includes the flow depth along the boundary at the time of peak flow. Additionl information can be found in (4) or the README files in each folder.

For beginners to Python and jupyter notebook:

The code is broken down into blocks. The first block includes module dependencies, which you must install before running the notebook in addition to jupyter notebook. The second block contains user-defined paths to the parflow data. The remaining blocks visualize the data.

To run the code, run each block sequentially. If you make changes to user preferences, you need to rerun only the block where you made changes and any subsequent blocks. Prior blocks should be unaffected.

References 

[1] Jones, J.E. and Woodward, C.S. (2001). Newton–Krylov-multigrid solvers for large-scale, highly heterogeneous, variably saturated flow problems. Advances in Water Resources, 24(7), 763–774, doi:10.1016/S0309-1708(00)00075-0.

[2] Ashby S.F. and Falgout, R.D. (1996). A Parallel Multigrid Preconditioned Conjugate Gradient Algorithm for Groundwater Flow Simulations. Nuclear Science and Engineering, 124(1), 145-159.

[3] Kollet, S.J. and Maxwell, R.M. (2006). Integrated surface-groundwater flow modeling: a free-surface overland flow boundary condition in a parallel groundwater flow model. Advances in Water Resources, 29(7), 945-958, doi:10.1016/j.advwatres.2005.08.006.

[4] CITATION FOR MY PAPER

[5] Maxwell, R.M. (2013) A terrain-following grid transform and preconditioner for parallel, large-scale, integrated hydrologic modeling. Advances in Water Resources, 53, 109-117, doi:10.1016/j.advwatres.2012.10.001.
