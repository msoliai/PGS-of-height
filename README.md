# Polygenic Score (PGS) Calculation Methods Notebook

## Overview

This notebook explores various methods for calculating Polygenic Scores (PGS). It provides a comprehensive workflow for PGS calculation, leveraging tools such as PLINK and R packages for genomic data analysis. The notebook includes data preprocessing steps, quality control, and multiple methods for PGS calculation.

## Requirements

### Software

To use this notebook, you need to have PLINK installed on your system. PLINK can be downloaded from the [PLINK website](https://www.cog-genomics.org/plink/). After downloading, make sure to add the PLINK executable to your system's PATH. This allows the notebook to call PLINK directly from any directory.

### R Environment

The notebook uses the `renv` package to manage R package dependencies. This ensures that all necessary packages are installed and the environment is consistent for all users. 

## Steps to Follow

### 1. Install PLINK

1. Download PLINK from [PLINK website](https://www.cog-genomics.org/plink/).
2. Extract the downloaded file to a directory of your choice.
3. Add the PLINK executable to your system's PATH. For example, you can add the following line to your `.bashrc` or `.zshrc` file:
   ```sh
   export PATH="/path/to/plink:$PATH"
   ```
   Replace `/path/to/plink` with the actual path to the PLINK directory.

### 2. Initialize R Environment

The notebook uses the `renv` package to create a reproducible R environment. When you run the notebook, it will initialize the `renv` environment and install all required packages.

After the `renv` environment is initiated, **you must reset the kernel** to apply the changes. This ensures that the notebook runs with the correct environment settings.

### 3. Set Project Directory

The notebook assumes that you have set the project directory as the root directory. There is code included in the notebook to help you ensure that the root directory is set correctly.

## Additional Information

- **Data Storage**: All input data files should be placed in the `data` directory. The notebook will read and write files to this directory. All required data files should be auto-downloaded into the data directory; I've made an effort to streamline this as much as possible. 
- **Temporary Files**: Intermediate files and outputs are stored in a temporary data directory (`tmp-data`). Ensure this directory exists or is created during the notebook execution.
- **Parallel Processing**: The notebook is designed to utilize multiple CPU cores for efficient data processing. Make sure your system supports multi-core processing and R is configured to use it.
- **Error Handling**: If you encounter any issues or errors, make sure all dependencies are installed correctly, and the paths are set properly. Check the notebook for any missing steps or additional configuration that might be required.

## Conclusion

This notebook provides a framework for calculating Polygenic Scores using various methods. By following the setup steps and ensuring your environment is correctly configured, you can efficiently analyze genomic data and derive meaningful insights from PGS calculations.

Feel free to contribute or modify the notebook to suit your specific needs.