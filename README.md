# Brain Tumor Segmentation using TransUNet

## Overview

This project presents a deep learning-based solution for brain tumor segmentation using the TransUNet architecture. The system integrates Convolutional Neural Networks (CNNs) with Vision Transformers to effectively capture both local spatial features and global contextual dependencies in MRI scans.

In addition to model development, a complete web-based interface has been implemented using Flask, enabling real-time visualization and prediction of tumor segmentation results.

---

## Dataset

* BraTS 2023 Dataset  
* Multi-modal MRI scans: T1, T1c, T2, FLAIR  

---

## Methodology

* MRI preprocessing (normalization, resizing, modality handling)  

* Implementation of:
  * UNet (baseline model)  
  * TransUNet (hybrid CNN + Transformer model)  

* Model training and evaluation using Dice Similarity Coefficient (DSC)  

* Comparative performance analysis  

---

## Results

* TransUNet Dice Score: **0.75**  

* TransUNet demonstrated improved segmentation accuracy over the baseline UNet model due to its ability to capture long-range dependencies  

---

## Sample Output

![Segmentation Result](sample_result/transunet_result.png)

---

## Web Application (Deployment)

A Flask-based web application was developed to make the model accessible through a user interface.

### Features

* Upload MRI scans  
* Perform segmentation  
* Visualize predicted tumor regions  

The application was tested using ngrok to enable external access and simulate real-world deployment.

---

## Project Structure

* notebook.ipynb → Model training and evaluation  
* sample_result/ → Sample predictions  
* models/ → Pretrained model download instructions  
* requirements.txt → Dependencies  

---



## Usage
* Run the notebook
* jupyter notebook notebook.ipynb
* Run Flask app
* python app.py
* Pretrained Models


## Technologies Used
* Python
* PyTorch
* NumPy
* Pandas
* Matplotlib
* Nibabel
* Flask
* Future Improvements
* Enhance Dice Score through hyperparameter tuning
* Extend to 3D segmentation
* Deploy on cloud platforms (AWS / GCP)

## Author

* Bilal Ahmed
* Bachelor of Science in Software Engineering

## Interests:
* Artificial Intelligence
* Medical Imaging
* Deep Learning

Due to GitHub size limitations, model weights are not included.

Download from:
https://drive.google.com/drive/folders/1NGUaJes5SfEilNXqjMjAB7kTMyB5MkgC

## Installation

```bash
pip install -r requirements.txt
