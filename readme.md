# Emotion Detection Project

This project implements emotion detection using deep learning models trained on the FER2013 dataset.

## Setup Instructions

### 1. Create a Virtual Environment

**For Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**For macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 2. Install Dependencies

Once the virtual environment is activated, install the required packages:

```bash
pip install -r requirements.txt
```

### 3. Dataset Setup

- Download the FER2013 dataset
- Extract it to the `fer2013` folder in the project root
- Ensure the folder structure is:
  ```
  fer2013/
  ├── train/
  │   ├── angry/
  │   ├── disgust/
  │   ├── fear/
  │   ├── happy/
  │   ├── neutral/
  │   ├── sad/
  │   └── surprise/
  └── test/
      ├── angry/
      ├── disgust/
      ├── fear/
      ├── happy/
      ├── neutral/
      ├── sad/
      └── surprise/
  ```

### 4. Run Training

Open and run the Jupyter notebook:

```bash
jupyter notebook notebooks/emotion_train.ipynb
```

## Project Structure

```
emotion_detection/
├── notebooks/
│   └── emotion_train.ipynb
├── fer2013/
│   ├── train/
│   └── test/
├── trained_models/
├── requirements.txt
└── readme.md
```

## Models

- **Baseline CNN**: Custom CNN architecture trained from scratch
- **ResNet18**: Transfer learning with fine-tuning on FER2013

## Requirements

- Python 3.8+
- PyTorch
- torchvision
- NumPy
- Matplotlib
- scikit-learn
- seaborn
- Jupyter Notebook
