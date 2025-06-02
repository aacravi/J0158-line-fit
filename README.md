# J0158-line-fit

Script *single_line_fit*:

A code to perform the fitting of single emission lines of the lensed quasar Q J0158-4325 and extract best fit parameters for multi-epochs observations. The fitting is based on PyQSOFit and adapted to this specific quasar. It takes as input the 1D spectra of image A and image B (from gravitaional lensing) for the given epochs of observation, the redshift of quasar, and the specific characteristics of the line to analyze: the rest wavelength, the line name, the wavelength range of its emission and if a narrow component must be included in the fitting. An affine fitting of the spectrum of image B on image A is performed, to check for microlensing bias. Finally, the parameters of the Guassian profiles used for the fitting are extracted and plotted against the time of observation. The outputs are:
- plot of the emission line for all epochs, for image A and B for quick visual comparison
- Plot of the affine fit of image B on image A, together with plot of residuals
- Fitting plots from PyQSOFit of all epochs, image A and B
- Plots of the extracted parameters against time of observation
- Dictionary containing all information about the fits are saved

Script *compare_2_lines*:

This script compares the extracted parameters from the line fitting of two different lines and tries fitting periodic functions to check for periodicity. This script should be run after running *single_line_fit* for the two lines to compare. 

In the folder *J0158 plots* are collected all the fitting plots for the lines MgII and H alpha.
