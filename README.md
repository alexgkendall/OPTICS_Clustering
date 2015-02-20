##OPTICS CLUSTERING##
This MATLAB function computes a set of clusters based on the algorithm introduced in Figure 19 of Ankerst, Mihael, et al. "OPTICS: ordering points to identify the clustering structure." ACM Sigmod Record. Vol. 28. No. 2. ACM, 1999.

**Written by Alex Kendall**
University of Cambridge
18 Feb 2015
http://mi.eng.cam.ac.uk/~agk34/

This software is licensed under GPLv3, see included glpv3.txt.

**Input:**

points - input points to cluster where each point is a separate row and the columns are data dimensions

minpts - the minimum points required to form a cluster

epsilon - a percentage threshold to make a cluster


**Output:**

SetOfClusters - a struct containing each cluster's start and end index

RD - each point's reachability distance

CD - each point's core distance

order - the order of points in the reachability graph


**Dependencies:**
This function requires optics.m from Michal Daszykowski's implementation of calculating the reachability distance for all points.
For more details, refer to http://chemometria.us.edu.pl/index.php?goto=downloads
