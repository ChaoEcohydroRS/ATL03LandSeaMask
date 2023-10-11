# ATL03LandSeaMask

[![DOI](https://zenodo.org/badge/678219089.svg)](https://zenodo.org/badge/latestdoi/678219089)
## Abstract
The NASA Ice, Cloud, and land Elevation Satellite 2 (ICESat-2) employs precise lasers to measure Earth's surface elevation through photon data. This data is particularly valuable in remote locations where traditional surveying methods are either expensive or less feasible. For example, it can reveal critical insights into ocean conditions globally. However, despite the availability of some methods for land/sea classification based on photon data, these techniques often require extensive efforts. The absence of a standardized method for transforming photon data into actionable land/sea measurements makes it difficult for both ocean and terrestrial communities, especially new users, to utilize ICESat-2 data.
To address this gap, we introduce SeaLandIdentifier, an open-source Python tool designed to simplify the process of labeling land/sea and extracting ICESat-2 data. By linking ICESat-2 photon data with existing updated high-resolution land-sea mask datasets, SeaLandIdentifier enables users to visualize photon returns alongside coincident shoreline data for accurate inspection. 
Our work aims to eliminate obstacles when scientists prepare high-resolution ICESat-2 data over land or sea. SeaLandIdentifier is expected to be a key tool for the development of future "Ancillary Masks" products for ICESat-2 data, thereby promoting more efficient and user-friendly land/sea classification.


## Overview
(A statement of need
The authors should clearly state what problems the software is designed to solve, who the target audience is, and its relation to other work.)

This is a repository for publishing “An Open-Source Tool for Updating ICESat-2 ATL03 Land-Sea Masks with High-Resolution Shoreline Datasets”

The ATL03LandSeaMask is a tool designed to Update ICESat-2 ATL03 Land Sea Mask with high-resolution shoreline dataset. This repository is home to the code and materials for the publication "An Open-Source Tool for Updating ICESat-2 ATL03 Land-Sea Masks with High-Resolution Shoreline Datasets."

## Main subject of the paper
The main subject of the paper is to develop and introduce an open-source tool named "SeaLandIdentifier". By integrating ICESat-2 photon data with high-resolution land-sea mask datasets, SeaLandIdentifier allows users to visualize and accurately inspect photon returns along shorelines. This work contributes to making ICESat-2 data more accessible and user-friendly for both ocean and terrestrial communities, and it is anticipated to be instrumental in the creation of future "Ancillary Masks" products for ICESat-2 data.
1) Processing ICESat-2 h5 Files: Sorting ICEsat-2 h5 files based on photon return signature, which is a unique characteristic of the light signal received by the satellite.
2) Landmask Application: Applying a landmask to h5 files to remove data points likely taken from land, enhancing the analysis of water bodies.
3) The paper discusses the methodology, implementation, and applications of this tool, providing insights into the enhancement of ICESat-2 data processing and analysis.

## Features

- **Processing ICESat-2 h5 Files**: The tool enables the sorting of ICEsat-2 h5 files based on photon return signature.
- **Landmask Application**: The application of a landmask to h5 files ensures that data points likely taken from land are removed, allowing for precise analysis of water bodies.

## Getting Started

To use this tool, follow the instructions below:

### 1) Prerequisites

- I used VS code python IDE as the working environment. We used jupyter notebook version for illustating how to use it. You can alwasy easily convert it to pipline.
- The global coastal shoreline dataset.

### 2) Installation

- Run conda env create -f environment.yml

### 3) Usage

- All steps in our work are presented in Jupyter Notebooks

## Support and Contribution

Feel free to open an issue if you encounter any problems or have any suggestions. Contributions are welcome!

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Citation
If you use this software in your research, please cite the associated paper using the DOI provided below.
Chao Wang, Emily Eidam, Tamlin Pavelsky, Kelsey Bisson, & Catherine Walker. (2023). An Open-Source Tool for Updating ICESat-2 ATL03 Land-Sea Masks with High-Resolution Shoreline Datasets (v1.0.2). Zenodo. https://doi.org/10.5281/zenodo.8245306

## Acknowledgments

- This research was funded by NASA's ICESat-2 Program (grant number: 80NSSC21K0914).
- We thanks Dr. Tyler Sutterley for the "icesat2_toolkit", we used some of his functions.
