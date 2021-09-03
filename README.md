Recreating Pleiades HR Diagram using dbscan algorithm from sklearn

Disclaimer: The goal of this code is to study how to recreate H-R Diagram of a stellar cluster (in this case Pleiades) using DBSCAN clustering algorithm from sklearn. I'm sorry if the method is not so scientific.

The data is downloaded from Gaia early data release 3 (Gaia Collaboration, 2020, Gaia EDR3, Version 1.0. https://doi.org/10.5270/esa-1ugzkg7). 
The data I'm using is downloaded from Gaia early data release 3 downloaded from https://gea.esac.esa.int/archive/

This notebook shows how to create an HR Diagram (Hertzsprung-Russel Diagram) or color-magnitude diagram of a stellar cluster. This works as the following
First, we download the data and then plot it in ra and dec. This shows a small patch of the sky.
Second, to identify the cluster we plot it in pmra and pmdec. This shows the proper motions of the stars in the cluster. A cluster of stars tend to move at the same velocity, we will see the cluster as a small clump that isolate themselves from the rest of the data.
Third, we use dbscan and use necessary parameters that characterize the cluster. Data with similar properties will be identified as the cluster.
Forth, after obtaining the cluster we plot them in their magnitude and spectrum/color.

In this notebook we can see the diagram we see the cluster has a straight diagonal line. This characterize an open cluster because the line shows the main sequence of the cluster, it means the stars in this cluster is still young.
