# Automating Waste Sorting with Deep Learning

This project uses a Convolutional Neural Network (CNN) to classify synthetic images of **plastic**, **paper**, and **garbage bags**. The model is built with TensorFlow/Keras and evaluated with Scikit-learn metrics.

---

## Dataset

The project uses a synthetic dataset of bag types available on Kaggle:

**[Plastic - Paper - Garbage Bag Synthetic Images](https://www.kaggle.com/datasets/vencerlanz09/plastic-paper-garbage-bag-synthetic-images)**

After downloading, structure the dataset as follows:

```
INPUT/
└── Bag Classes/
    ├── Plastic/
    ├── Paper/
    └── Garbage/
```

Each folder should contain image files (`.jpg`) of the corresponding class.

## Requirements

The project depends on the following packages:

- `matplotlib`
- `numpy`
- `pandas`
- `Pillow`
- `scikit-learn`
- `tensorflow`

### Install via `requirements.txt`:

```bash
pip install -r requirements.txt
```

Or with Conda:

```bash
conda create -n cnn python=3.10
conda activate cnn
pip install -r requirements.txt
```

---

## How to Run

1. **Download and extract the dataset** as shown above.

2. **Install the dependencies**.

3. **Open and run the Jupyter Notebook**:

```bash
jupyter notebook main.ipynb
```

4. **File dialog**: The script uses a GUI (tkinter), a file picker will appear for image selection.

---

## Features

- CNN built with TensorFlow/Keras
- Dataset loading from structured folders
- Train-test split and metric evaluation
- Visualizations: confusion matrix, ROC curve
- GUI integration with `tkinter` for interactive file selection

---

## Notes

- The dataset directory must be present at `INPUT/Bag Classes/`.
- All classes must have their own subfolders.

---
