# BraTS 2020: Brain Tumor Segmentation and Survival Prediction

This repository contains Jupyter Notebooks for building machine learning/deep learning pipelines to perform 3D Brain Tumor Segmentation and Predict Patient Survival using the BraTS 2020 (Brain Tumor Segmentation Challenge 2020) dataset.

## Team members
No.NameStuIDWork1Nguyễn Tất Kiên2311735- Handle model API and architecture- Training models & logging- Hyperparameters Tuning2Nguyễn Thành Minh Khôi2311687- Data exploration- Data preprocessing- Data augmentation3Nguyễn Lâm Huy2311188- Feature Engineering- Evaluation- Models Comparing

## Project Structure

* **`brats_segmentation_training.ipynb`**: This notebook contains the data preprocessing, model building, and training pipeline for 3D brain tumor segmentation. It typically involves building 3D U-Net or similar architectures to segment different tumor sub-regions (e.g., ET, WT, TC) from multi-modal MRI scans (T1, T1ce, T2, FLAIR).
* **`BraTS_Survival_Prediction.ipynb`**: This notebook focuses on predicting the overall survival (in days) of patients. It utilizes clinical data (like age) combined with extracted radiomic features or deep learning-based features from the tumor segmentations to build regression or classification models.

## Dataset

The data used for this project is from the [BraTS 2020 Challenge](https://www.kaggle.com/datasets/awsaf49/brats20-dataset-training-validation). 
* The training dataset contains multi-modal MRI scans for predicting brain tumor segmentation.
* Clinical data is provided for a subset of the dataset to predict patient overall survival.

## Getting Started

### Prerequisites

You will need Python 3.x and standard data science and deep learning libraries, typically including:
* PyTorch
* NumPy
* Pandas
* SimpleITK / NiBabel (for reading `.nii` or `.nii.gz` medical imaging files)
* Matplotlib / Seaborn
* Scikit-Learn

### Usage

1. Clone this repository.
2. Download the BraTS 2020 dataset and place it in the appropriate data directory (you may need to configure data paths within the notebooks).
3. Run `brats_segmentation_training.ipynb` to train the segmentation model and visualize predictions.
4. Run `BraTS_Survival_Prediction.ipynb` to train the survival prediction model based on extracted features and patient clinical data.

## Acknowledgments

* [MICCAI BraTS Challenge](http://braintumorsegmentation.org/)
