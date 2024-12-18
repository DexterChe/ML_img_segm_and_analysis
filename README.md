# Machine Learning Image Segmentation and Particle Analysis

This repository contains code and analysis related to **image segmentation** using machine learning techniques applied to **analysis of ferroelectric domain**. The main focus is segmenting particles in microscopy images, extracting their geometrical features, and conducting a detailed statistical analysis.

## Project Overview

The goal of this project is to automate the detection and segmentation of domains/particles from **SEM (Scanning Electron Microscopy)** images and extract their geometrical parameters (e.g., size, shape). Afterwards, the data is used to perform statistical analysis, including size distribution, regression models, and advanced visualizations.

#### Example of the image
| Original image | Segmented image |
|:--------------:|:---------------:|
| ![Original image](https://raw.githubusercontent.com/DexterChe/ML_img_segm_and_analysis/main/image_example/D50_10kV_1_row_005.png) | ![Segmented image](https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/D50_10kV_1_row_005%20Segmented.png) |

#### Assess of particle segmentation quality
![Assess of particle segmentation quality](https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/1_DF25_600pA_005_FastSAM_s_result_crop_compare_2.png)

#### Distributions
<div style="display: flex; justify-content: space-between;">
  <img src="https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/KDE_for_doses.png" alt="Bar plot A vs currents" width="45%"/>
  <img src="https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/KDE_for_currents.png" alt="Bar plot A vs dose factor" width="45%"/>
</div>

#### Analysis
<div style="display: flex; justify-content: space-between;">
  <img src="https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/Bar_plot_A_vs_dose_factor.png" alt="Bar plot A vs dose factor" width="45%"/> 
  <img src="https://github.com/DexterChe/ML_img_segm_and_analysis/blob/main/examples_results/Bar_plot_A_vs_currents.png" alt="Bar plot A vs currents" width="45%"/>
</div>


### Key Features:
- **Image Segmentation**: Machine learning techniques are used to detect particles in SEM images.
- **Data Extraction**: Geometrical features such as size and shape are extracted from segmented images.
- **Statistical Analysis**: Performs statistical analysis of particle sizes, including size distributions, regression analysis, and visualization through histograms, violin plots, and more.
- **Automation**: Automates the entire pipeline from segmentation to data analysis.

## Project Structure

- `ML_image_segmentation.ipynb`: Jupyter Notebook implementing image segmentation using machine learning models.
- `PSD_analysis_annealed_regress.ipynb`: Jupyter Notebook performing particle size distribution analysis and regression on extracted data.
- `LICENSE`: GNU Affero General Public License, Version 3.

## Getting Started

### Prerequisites

- **Python 3.8+**
- **Jupyter Notebook**
- Libraries: `scikit-learn`, `opencv-python`, `matplotlib`, `pandas`, and more (refer to the notebooks for specific dependencies).

### Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/DexterChe/ML_img_segm_and_analysis.git
    ```

2. Install the necessary Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Open and run the provided Jupyter notebooks:
    - For image segmentation: `ML_image_segmentation.ipynb`
    - For data analysis and regression: `PSD_analysis_annealed_regress.ipynb`

## Example Data

A folder named `image_example` contains sample SEM images used for segmentation and analysis. You can replace these images with your own SEM images for custom analysis. A folder named `examples_results` contains examples of results: segmented images, KDE plots and bar plots.

## Future Enhancements

- Integration of more advanced machine learning models for enhanced segmentation accuracy.
- Expanded statistical analysis, including other types of visualizations and data correlations.
- Potential integration with data visualization platforms like **Power BI**.

## License

This project is licensed under the GNU Affero General Public License, Version 3. See the [LICENSE](LICENSE) file for more details.

## Contact

For any inquiries, feel free to contact:
- GitHub: [DexterChe](https://github.com/DexterChe)
