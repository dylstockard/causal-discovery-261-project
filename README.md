# causal-discovery-261-project
Repository for the 261 project "Causal Discovery for Aerosol-Cloud Interactions" by Giorgia Nicolaou, Dylan Stockard, and Shobhit Dronamraju

This repository contains the code used to generate our artifical data with a known causal graph structure and non-linear, non-gaussian error term, code to run each of our tested algorithms, and the two datasets we tested upon.

### data_generator.ipynb
This python notebook contains the code for two things. First, it generates artificial data. The first main cell generates the artifical dataset to have similar dimensions and structure as the Aerosol cloud data we tested the models on. This means generating multiple variables with random known causal connections that vary to see which were easiest and which were hardest to find. Second, the other large cell is re-formatting the data for the TCDF experiments since that model required the data to be in a new format that required heavier pre-processing.

### cmiknn_version.py
The script to run LPCMCI (CMIknn version). This is one of our conditional-independence based methods.

### parcorr_version.py
The script to run LPCMCI (ParCorr version). This is one of our conditional-independence based methods.

### Dynotears-sim.ipynb
The notebook to run DynoTears. This is our algorithmic method based on NoTears.

### runTCDF.py
The script to run TCDF. This is our CNN method.

### VARLiNGAM.ipynb
The notebook to run VARLiNGAM. This is our LiNGAM method.

### aerosol_cloud_data.csv
Our novel test data with unknown causal connections and non-linear non-gaussian error terms.

### simulated_updated_no_index.csv
Our simulated test data with known causal connections generated from `data_generator.ipynb`
