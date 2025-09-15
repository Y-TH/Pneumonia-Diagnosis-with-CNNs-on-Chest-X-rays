# Pneumonia Diagnosis with CNNs on Chest X-rays

## Project Overview
This repository contains a computer vision project for classifying chest X-ray images as **Pneumonia** or **Normal** using Convolutional Neural Networks (CNNs) implemented in PyTorch.  
The goal is to build a model capable of assisting automated diagnosis of pneumonia from chest X-ray images.

---

## Dataset
The dataset is publicly available on [Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) and contains **5,863 JPEG images** divided into 2 categories: `PNEUMONIA` and `NORMAL`.

It is organized into three main sets:
- `train/` — Training images  
- `val/` — Validation images  
- `test/` — Test images  

Each set contains subfolders for each image category (`PNEUMONIA` and `NORMAL`).  

**Note:** The dataset is **not included** in this repository due to size. After downloading, place it inside the `data/` folder as shown:
```
pneumonia-diagnosis/
└── data/
    ├── train/
    ├── val/
    └── test/
```

Optional subfolders like `__MACOSX` can be ignored.

**Dataset Credit:**  
- Author: Paul Mooney  
- Source: [Mendeley Data](https://data.mendeley.com/datasets/rscbjbr9sj/2)  
- License: CC BY 4.0  

---

## Environment Setup
This project uses **Conda** for environment management. To create the environment and install dependencies:

```bash
# Create conda environment with Python 3.9
conda create -n pneumonia-env python=3.9
conda activate pneumonia-env

# Install packages from requirements.txt
pip install -r requirements.txt
```

---

## Project Structure
```
pneumonia-diagnosis/
├── data/           # Dataset folder (not included)
├── notebooks/      # Jupyter notebooks for exploration & experiments
├── src/            # Source code for model training and evaluation
├── models/         # Saved trained models
├── README.md       # Project description and instructions
├── requirements.txt# Python dependencies
├── .gitignore      # Ignored files/folders (data, envs, etc.)
└── LICENSE         # MIT License
```

---

## Usage
1. **Download the dataset** from Kaggle and place it in `data/`.
2. **Activate the environment:**
```bash
conda activate pneumonia-env
```
3. **Install dependencies:**
```bash
pip install -r requirements.txt
```
4. **Run notebooks or scripts** in `notebooks/` or `src/` to train, validate, and evaluate the CNN model.

---

## License
This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements
* Kaggle dataset author: Paul Mooney
* PyTorch community for model implementation references
