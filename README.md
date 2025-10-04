# Overview

YonedaRRE is a Github repository that provides the source code of the "Study on the Anomalous ”Yoneda” Reflection Below Specular Reflection in Highly Absorptive X-Ray Regimes" paper. This repository consists of three main notebooks. "Generates-Data.ipynb" and "Generate-Figures.ipnyb" are used the reproduce all data and figures presented in the paper. RRE.ipynb is general code that can be modified to do the similar calculations for any other material, provided that its refractive index data has been retrieved from The Center of X-Ray Optics (CXRO) website.

# Requirements

All programs are written in Python. Ensure that you have at least Python 3.11 with pip and venv installed. The following external packages are required to run the programs:
- numpy, for numerical calculations.
- matplotlib, for plotting.

Additionally, the SciencePlots package is utilized as the matplotlib scientific plotting styles. A latex compiler is necessary to implement this plotting style package. For a more detailed installation guide, please refer to: https://github.com/garrettj403/SciencePlots.

Once all prerequisite packages have been installed, clone this repository with the command:
```
git clone https://github.com/NabailAzhiim/YonedaRRE.git
```
Then move into the repository directory
```
cd YonedaRRE
```

# Reproducing Figures

## Generating data

Make sure "Al.dat" and "Cu.dat" files are available. These files contains the refractive index data of Al and Cu retrieved from the CXRO website. After that, run all of the in "Generate-Data.ipynb". This will create additional "Al" and "Cu" folders to store all calculation results. 

## Generating figures

Open "Figures" folder and you will find Fig. 3 in the paper that depicts the illustration of the scattering problem and polarization convention. To reproduce the rest of the figures, simply run all of the cells in "Generate-Figures.ipynb". Note that all figures are saved as a pdf file. 

# The Similar Calculations for Other Material

To do this, first we need to determine which materials we want to analyze and then retrieve the refractive index data from the CXRO website. If you are not familiar with this website, please refer to "How to Retrieve Refractive Index Data.pdf" for the more detailed guidance. Make sure you save the refractive index data as a "sample.dat" file. After that, open "RRE.ipynb" and read the description of each cell in that notebook. You may refer to "Generate-Data.ipynb" if you need some examples on how to run the calculations.