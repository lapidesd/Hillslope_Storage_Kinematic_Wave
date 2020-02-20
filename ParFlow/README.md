# ParFlow simulations: supplementary data and code

This directory includes folders containing results from numerical simulations with ParFlow (1,2,3,5) on divergent/convergent hillslopes with exponential width functions (w = ce^(ax) ) as described by (4). The values of a range from -0.1 (very convergent) to 0.1 (very divergent). Content included is as follows:

* Boundary_flow_data: Boundary flow data in this folder contain overlandsum output from ParFlow simulations on curved hillslopes (convergent or divergent) as described in Lapides et al. (2020). All hillslopes are 50m long, but the widths vary depending on the curvature since hillslope area is kept at a constant 3000 m2 for all simulations. Each file contains data from a separate simulation, and the value of a (the curvature parameter for the exponential width function w = ce^(ax) ) is given by the number at the beginning of the file name. Positive values of a indicate divergent hillslopes, and negative values of a indicate convergent hillslopes. Some files indicate a resolution. The resolution is given as 4, 2, 1, 0.5, or 0.25. The temporal and spatial meaning of these resolutions is given in Lapides et al. (2020). Data are reported by "index," which is the location along the bottom boundary in relation to the center of the hillslope. The column "value" reports the overlandsum value at each cell along the hillslope boundary during the equilibrium peak flow portion of the hydrograph.
* Flow_depth: Flow depth data in this folder contain flow depths from ParFlow simulations on curved hillslopes (convergent or divergent) as described in Lapides et al. (2020). All hillslopes are 50m long, but the widths vary depending on the curvature since hillslope area is kept at a constant 3000 m2 for all simulations. Each file contains data from a separate simulation, and the value of a (the curvature parameter for the exponential width function w = ce^(ax) ) is given by the number at the beginning of the file name. Positive values of a indicate divergent hillslopes, and negative values of a indicate convergent hillslopes. Some files indicate a resolution. The resolution is given as 4, 2, 1, 0.5, or 0.25. The temporal and spatial meaning of these resolutions is given in Lapides et al. (2020). Data are reported by "index," which is the location along the bottom boundary in relation to the center of the hillslope. The column "value" reports the depth at each cell along the hillslope boundary during the equilibrium peak flow portion of the hydrograph.
* Hydrograph_data: Hydrograph data in this folder contain overlandsum output from ParFlow simulations on curved hillslopes (convergent or divergent) as described in Lapides et al. (2020). All hillslopes are 50m long, but the widths vary depending on the curvature since hillslope area is kept at a constant 3000 m2 for all simulations. Each file contains a separate hydrograph, and the value of a (the curvature parameter for the exponential width function w = ce^(ax) ) is given by the number at the beginning of the file name. Positive values of a indicate divergent hillslopes, and negative values of a indicate convergent hillslopes. Some files indicate a resolution. The resolution is given as 4, 2, 1, 0.5, or 0.25. The temporal and spatial meaning of these resolutions is given in Lapides et al. (2020). Data are reported by "index," which is the timestep in ParFlow. The time increment used is 0.5 seconds, and the hydrographs reported in the column "sum" are total flow along the bottom boundary. The columns "SD" and "mean" contain the standard deviation and mean flow across the boundary, respectively.
* Parflow_Visualization.ipynb: jupyter notebook that visualizes each type of data provided in the data directories including: hydrograph data, boundary flow data, and boundary depth data. Additional blocks show the differences between simulations run at different resolutions.


For beginners to Python and jupyter notebook:

The code is broken down into blocks. The first block includes module dependencies, which you must install before running the notebook in addition to jupyter notebook. The second block contains user-defined paths to the parflow data. The remaining blocks visualize the data.

To run the code, run each block sequentially. If you make changes to user preferences, you need to rerun only the block where you made changes and any subsequent blocks. Prior blocks should be unaffected.

References 

[1] Jones, J.E. and Woodward, C.S. (2001). Newton–Krylov-multigrid solvers for large-scale, highly heterogeneous, variably saturated flow problems. Advances in Water Resources, 24(7), 763–774, doi:10.1016/S0309-1708(00)00075-0.

[2] Ashby S.F. and Falgout, R.D. (1996). A Parallel Multigrid Preconditioned Conjugate Gradient Algorithm for Groundwater Flow Simulations. Nuclear Science and Engineering, 124(1), 145-159.

[3] Kollet, S.J. and Maxwell, R.M. (2006). Integrated surface-groundwater flow modeling: a free-surface overland flow boundary condition in a parallel groundwater flow model. Advances in Water Resources, 29(7), 945-958, doi:10.1016/j.advwatres.2005.08.006.

[4] CITATION FOR MY PAPER

[5] Maxwell, R.M. (2013) A terrain-following grid transform and preconditioner for parallel, large-scale, integrated hydrologic modeling. Advances in Water Resources, 53, 109-117, doi:10.1016/j.advwatres.2012.10.001.
