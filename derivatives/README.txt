Preprocessing Steps:

The following preprocessing steps were applied to the raw functional data:

1. MEICA preprocessing pipeline (version 3.2 beta):
1.1. Removal of the first four volumes
1.2. Normalization to the MNI template
1.3. Optimal combination across echo times
1.4. ICA-based denoising

2. Resampling to 2.5 mm isotropic voxels using FSL (version 6.0.6.5).

3. Spatial smoothing with a 6 mm Gaussian kernel using FSL SUSAN.

-----------------------

Stimulus Onset Correction:

To adjust stimulus onsets, subtract 12 seconds (i.e., 4 TR × 3 sec/TR) from the onset times provided in the events files of the raw dataset.