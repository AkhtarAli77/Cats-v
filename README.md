## Submitted by:
## Name:    Akhatar Ali
## Roll NO.: 202210101150139
## Course:B.Tech. CS(DS+AI)
## Group: 75
## Subject: Deep Learning
## Subject Code: UCS7802
## Submitted to: Mr. Angshuraj Gharami
# Classification of Cats and Dogs using CNN

This project demonstrates how to build, train, and evaluate a Convolutional Neural Network (CNN) to classify images of cats and dogs. The entire workflow—from data loading and preprocessing to model training and evaluation—is implemented in a single Jupyter Notebook.

## Table of Contents
- Project Overview
- Notebook
- Dataset
- Model Summary
- Preprocessing & Augmentation
- Training & Evaluation
- Usage (Run instructions)
- Requirements
- Tips for improving performance
- Project structure
- Contributing
- License
- Contact & Acknowledgements

## Project Overview
This project demonstrates an end-to-end workflow for classifying images of cats and dogs using a Convolutional Neural Network (CNN). Built with TensorFlow and Keras, the project covers all major steps in an image classification pipeline, including data loading, preprocessing, augmentation, model design, training, evaluation, and predictions.

The goal of this project is to provide a clear, beginner-friendly example of how to build a deep learning model for binary image classification. All code and explanations are contained in a single Jupyter Notebook, making it easy to follow, modify, and experiment with different settings.

## Notebook
The main implementation of this project is available in a single Jupyter Notebook:

Cats-vs-Dogs-CNN.ipynb

Open this notebook to:

Explore the complete step-by-step workflow

Modify hyperparameters

Visualize training graphs and evaluation metrics

Reproduce model training and predictions

The notebook is fully self-contained and easy to run on both local systems and Google Colab.

## Dataset
This project is intended to use the popular Kaggle "Dogs vs Cats" dataset:
- Kaggle competition / dataset: https://www.kaggle.com/datasets/alvarole/asirra-cats-vs-dogs-object-detection-dataset
- Google Dive Link / dataset:   https://colab.research.google.com/drive/1tuqjaAiJnjMAib7TrZI_trTFQY2yPw7G#scrollTo=972on1TNVfPR

Notes:
- The dataset must be downloaded separately (Kaggle requires authentication). Place the images in the paths expected by the notebook (instructions are included inside the notebook).
- For quick experimentation you can use a smaller subset or sample a limited number of images per class.

## Model Summary
The project uses a custom Convolutional Neural Network (CNN) designed for binary image classification (Cats vs Dogs). The model includes:

Convolutional Layers (Conv2D): Extract spatial features such as edges, patterns, and textures.

ReLU Activation: Introduces non-linearity for better learning.

MaxPooling Layers: Reduce spatial dimensions and help capture important features.

Dropout Layers: Prevent overfitting by randomly disabling neurons during training.

Flatten Layer: Converts feature maps into a 1D vector before passing to dense layers.

Dense Layers: Learn high-level patterns for classification.

Output Layer: Uses a sigmoid activation for binary output (cat or dog).

The architecture is simple, efficient, and achieves high accuracy on the Cats vs Dogs dataset. It can also be easily extended with advanced techniques such as batch normalization or transfer learning.

## Preprocessing & Augmentation
This project uses Keras ImageDataGenerator to prepare the images before training.

Preprocessing includes:

Resizing all images to a fixed size

Normalizing pixel values (0–1)

Augmentation includes:

Rotation

Zoom

Shifts

Horizontal flip

These steps help reduce overfitting and improve model accuracy.

## Training & Evaluation
-The model is trained using Binary Crossentropy and the Adam optimizer. Accuracy and loss are tracked during training. After training, the model is evaluated using validation accuracy, a confusion matrix, and sample predictions.
## Usage (Run instructions)

1. Clone the repository
   - git clone https://github.com/AkhtarAli77/Cats-v/blob/main/cat-vs-dog.ipynb

2. Download the Dogs vs Cats dataset from Kaggle and place it where the notebook expects.
   - Dataset:https://www.kaggle.com/datasets/alvarole/asirra-cats-vs-dogs-object-detection-dataset
   - Google Dive Link / dataset: https://colab.research.google.com/drive/1tuqjaAiJnjMAib7TrZI_trTFQY2yPw7G#scrollTo=972on1TNVfPR

3. Install dependencies (example using pip)
   - python -m pip install --upgrade pip
   - pip install -r requirements.txt
   If a requirements file is not present, install the typical packages below.

4. Start Jupyter Notebook / JupyterLab
   - jupyter notebook
   - or
   - jupyter lab

5. Open and run the notebook `Classification-of-Cats-and-Dogs.ipynb`. Follow prompts in the notebook (paths, training duration, GPU usage).

Notes for Colab:
- If you prefer Google Colab, upload the notebook and mount your Google Drive (or use Kaggle API to download the dataset directly in the Colab runtime). Enable GPU in Runtime > Change runtime type.

## Requirements
Typical packages used by the notebook:
- Python 3.8+
- jupyter
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- tensorflow (>=2.0) or tensorflow-gpu
- keras (if using standalone Keras; otherwise use tensorflow.keras)
- pillow (PIL)
- opencv-python (optional, if used for image ops)

Example pip install:
```
pip install jupyter numpy pandas matplotlib seaborn scikit-learn tensorflow pillow
```

(If a requirements.txt file is present in the repo, use that.)

## Tips for improving performance
Use transfer learning models like MobileNet or EfficientNet

Add batch normalization or dropout

Increase data augmentation

Train for more epochs with early stopping

Use a GPU for faster training

## Project structure
- /Cats-vs-Dogs-CNN
│
├── Cats-vs-Dogs-CNN.ipynb     # Main notebook
├── data/                      # Dataset folder (user-provided)
├── requirements.txt           # Dependencies file (optional)
└── README.md                  # Project documentation


## Contributing
Contributions are welcome!
You can help by improving the notebook, enhancing the model, adding new features, or fixing issues.
To contribute, simply open an issue or submit a pull request.

## License
This repository is provided under the MIT License. See the LICENSE file for details (if included).

## Contact & Acknowledgements
- Author: Akhatar Ali
- Acknowledgements: Kaggle for the Dogs vs Cats dataset and the many open-source libraries used (TensorFlow, Keras, scikit-learn, etc.).



