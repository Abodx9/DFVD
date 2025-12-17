# DFVD

### Overview

DFVD is a voice classification project that distinguishes between real and synthetic (AI-generated) human voices. The system uses pretrained Wav2Vec2 models to extract speech embeddings and trains multiple classifiers including a neural network, XGBoost, and LightGBM to detect deepfake audio with high accuracy.

The repository includes training notebooks, model definitions, and inference scripts to extract embeddings and evaluate unseen audio samples.


## Features

* Extracts high-quality speech features using Wav2Vec2 (Facebook’s wav2vec2-xls-r-300m).
* Trains and evaluates three classifiers:

  * Simple feed-forward neural network
  * XGBoost gradient boosting model
  * LightGBM gradient boosting model
* Unified inference pipeline to compare model predictions.
* Modular and extensible architecture for adding new models or datasets.

---

## Repository Structure

```
DFVD/
├── Models/                     # Saved trained models
├── Training Notebook/          # Notebooks for training models
├── examples/                   # Example audios
├── Loader.ipynb                # Demo loader notebook
├── README.md                   # Project overview
├── .gitignore
├── LICENSE
```

---

## Requirements

To run training or inference code you will need:

* Python 3.10+
* PyTorch
* Transformers
* XGBoost
* LightGBM
* Librosa
* SoundFile
* Scikit-learn
