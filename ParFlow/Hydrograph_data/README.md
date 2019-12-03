
Hydrograph data in this folder contain overlandsum output from ParFlow simulations on curved hillslopes (convergent or divergent) as described in Lapides et al. (2020). All hillslopes are 50m long, but the widths vary depending on the curvature since hillslope area is kept at a constant 3000 m2 for all simulations. Each file contains a separate hydrograph, and the value of a (the curvature parameter for the exponential width function w = ce^(ax) ) is given by the number at the beginning of the file name. Positive values of a indicate divergent hillslopes, and negative values of a indicate convergent hillslopes. Some files indicate a resolution. The resolution is given as 4, 2, 1, 0.5, or 0.25. The temporal and spatial meaning of these resolutions is given in Lapides et al. (2020). 

Data are reported by "index," which is the timestep in ParFlow. The time increment used is 0.5 seconds, and the hydrographs reported in the column "sum" are total flow along the bottom boundary. The columns "SD" and "mean" contain the standard deviation and mean flow across the boundary, respectively.

Hydrographs can be visualized using the jupyter notebook XXXX.ipynb in the parent directory.

Lapides, etc. CITATION GOES HERE.
