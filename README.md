# R codes for matrixNS
Last update: 22 Jun 2026

This code is provided to reproduce the experimental results found in the main text and supplementary material of the paper "Graph estimation based on neighborhood selection for matrix-variate data"(matrixNS), which is scheduled for publication in the Journal of Multivariate Analysis (JMVA).

## Usage

To execute the code, please download and unzip all the included files into a single directory. Then run the R script corresponding to the figure or table you wish to reproduce:

- For Figure 5, Figure 6, and Table 2, run `matrixNS_realdata.R`.
- For all other figures and tables, run the script whose name matches the corresponding figure or table number.

**Note:** `matrixNS_supp_fig5.R` requires `matrixNS_fig3.R` to be run first.

Minor differences from the results reported in the paper may arise due to differences in the random seed.

## Working directory

This code uses the `here` package to set the working directory and load source files. If the `here` package does not work properly in your environment, please manually set the working directory to the directory where all the included files are saved.

## EEG data for the real data analysis

The EEG database used for the real data analysis in Section 5 is available at https://archive.ics.uci.edu/dataset/121/eeg+database. To prepare the data, please follow these steps:

1. Unzip the downloaded `eeg+database.zip` and the `smni_eeg_data.tar` file contained within it.
2. Create a folder named `eegsample` in the directory where your R codes are saved.
3. From the `smni_eeg_data` folder, extract the three files `c_m_co2c0000337.tar`, `c_n_co2c0000337.tar`, and `c_1_co2c0000337.tar`, and save their contents into the `eegsample` folder.

Alternatively, you may save the three files above in any directory of your choice and modify the file paths in `matrixNS_realdata.R` accordingly. However, if you prefer not to modify the code, we recommend following the steps above.

**Source:** Begleiter, H. (1995). EEG Database [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5TS3D.

## Contact

If you have any questions about the code, please contact: jpoth1729@snu.ac.kr
