# Related Software Packages

Here we list software packages that are related to the OpenSense ecosystem. Some of these packages provide complementary functionalities which is not available within the OpenSense ecosystem, while others provide similar functionalities that have been integrated into the OpenSense ecosystem and can thus be regarded as legacy software.

## Complementary Software

### pyNNcml

`pyNNcml` https://github.com/haihabi/PyNNcml is a software package for processing of CML and SML data with a focus on neural network-based methods.

### RainfallQC

`RainfallQC` https://github.com/NERC-CEH/RainfallQC provides quality control tools for rain gauge data. It implements the filters from the Global Sub-Daily Rainfall Quality Control (GSDR-QC) and also allows to call methods from `pypwsqc`.

### titanlib

`titanlib` https://github.com/metno/titanlib is a library of automatic quality control routines for weather observations, with an emphasis on spatial checks suitable for dense observation networks such as citizen weather observations.

## Legacy Software (methods integrated into the OpenSense ecosystem)

### RAINLINK

`RAINLINK` https://github.com/overeem11/RAINLINK is a collection of R scripts and functions for processing of CML data, focusing on 15-minute min-max data. It holds the original implementation of the nearby-link method which was integrated into `pycomlink`.

### PWSQC

`PWSQC` https://github.com/LottedeVos/PWSQC provides quality control for rainfall observations of PWS, implemeting the faulty zero, high influx and station outlier filter, which are now part of `pypwsqc`.

### pws-pyqc

pws-pyqc https://github.com/AbbasElHachem/pws-pyqc provides quality control and bias correction for PWS data using the indicator-based filter and bias correction which have been integrated into `pypwsqc`.