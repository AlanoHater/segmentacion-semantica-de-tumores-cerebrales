# Semantic Segmentation of Brain Tumors

## Project Description
This repository contains a Deep Learning project focused on the semantic segmentation of brain tumors from medical images (likely MRI scans). The core objective is to develop and train a robust Convolutional Neural Network (CNN), often based on architectures like U-Net, to achieve accurate pixel-wise classification and delineation of different tumor sub-regions (such as the necrotic core, peritumoral edema, and active tumor). The project aims to improve diagnostic precision and support treatment planning.

## 🎯 Project Goal
The primary goal is to implement and optimize a semantic segmentation model that can accurately map tumor components, achieving high scores on metrics like the Dice Coefficient and IoU (Intersection over Union).

## 📁 Repository Contents
The repository structure primarily consists of Jupyter notebooks detailing the model development pipeline:

* `Dataset.txt`: Provides information or source links for the medical imaging dataset used (e.g., data format, licensing, source challenge like BraTS).
* `Transfer_Learning.ipynb`: Explores the application of transfer learning techniques, using weights from pre-trained models to accelerate convergence and potentially improve segmentation results.
* `Version_2.ipynb`, `Version_3.ipynb`, `Version_4.ipynb`: Iterative notebooks documenting the development process, including different model configurations, data augmentation strategies, and hyperparameter tuning experiments.
* `untitled0.py`: Contains utility functions or preliminary code for data handling or model definition.

## 🧠 Methodology
The models employ an encoder-decoder architecture typical for semantic segmentation tasks (e.g., U-Net).

1.  **Architecture:** Implementation of a U-Net or similar FCN (Fully Convolutional Network).
2.  **Training:** Utilizes medical imaging data, often requiring specialized data loaders and augmentation routines (rotation, flipping, contrast adjustments).
3.  **Optimization:** Experimentation with various loss functions suitable for segmentation (e.g., Dice Loss, Focal Loss).
4.  **Evaluation:** Performance is primarily measured using the **Dice Coefficient** (F1 Score) and **IoU**.

## 🚀 Getting Started

### Prerequisites
* Python 3.x
* Deep Learning Framework (e.g., TensorFlow, Keras, or PyTorch)
* Standard scientific computing libraries (NumPy, Matplotlib)
* Specific medical image processing libraries (e.g., NiBabel, SimpleITK, depending on data format).

### Installation
1.  Clone the repository:
    ```bash
    git clone <repository-url>
    cd segmentacion-semantica-de-tumores-cerebrales
    ```
2.  (Recommended) Create and activate a virtual environment.
3.  Install dependencies (a `requirements.txt` is recommended):
    ```bash
    pip install tensorflow numpy matplotlib jupyter
    ```

### Usage
Navigate through the Jupyter notebooks in chronological order (`Version_2`, `Version_3`, `Version_4`, `Transfer_Learning`) to reproduce the experiments, train the models, and view the segmentation results.
