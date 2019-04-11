# Hillslope Storage Kinematic Wave
Programs to run the solution to the Hillslope Storage Kinematic Wave Equation for Overland Flow described by Lapides et al. n.d. (full citation below)

The jupyter notebook titled: Hillslope_storage_KW_analytic includes the solution to the hillslope-storage kinematic wave equation for overland flow for a width function described by an exponential of the form w=ce^(ax), where w is the contour width, i.e. distance between limiting streamlines, x is the distance downhill from the divide, a is a constant describing hillslope convergence/divergence, and c is a constant describing the size of the hillslope in the cross-slope direction. The jupyter notebook runs this solution for user-defined values of a, c, rainfall rate r, storm length tr, infiltration rate f, roughness parameter alpha, and hillslope length (xend-xtop, where xend is the outlet location and xtop is the divide location). The notebook produces characteristic nets for the storms as well as hydrographs of q or Q, depending on user preference. The program also prints the value of tc and qmax for each run.

A table of variables used in the code is included in this repository as well.

For beginners to Python and jupyter notebook:

The code is broken down into 4 different blocks. The first block includes module dependencies, which you must install before running the notebook in addition to jupyter notebook. The second block contains the equations described by Lapides et al. n.d.. The third block solves for characteristic nets and hydrograph data and plots the characteristic nets. This block includes a number of different options that users can change, commented in the code. The final block plots a hydrograph of q or Q depending on user preference. User-defined parameters are marked at the top of the block. 

To run the code, run each block sequentially. If you make changes to user preferences, you need to rerun only the block where you made changes and any subsequent blocks. Prior blocks should be unaffected.


CITATION FOR PAPER
