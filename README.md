# Data-Free Adversarial Attacks on DL Models in SDN-IoT Networks

This project explores **data-free adversarial attacks** on **Deep learning-based Autonomous anomaly detection** in **SDN** (Software Defined Network)-**IoT**(Internet of Things) networks. We analyse their impact on **CNN**, **LSTM**, and **AE-LSTM** models using **CICIDS2017**, **InSDN**, and **CICIOT23** datasets.

## Datasets Used

Datasets are **not included** in this repo due to size. Please download them manually from this Google Drive to have the same datasets as mine (CICIOT is lighter in my version) :

https://drive.google.com/drive/folders/1fIr_AWhk0C5NczuGIiSCrZBtUpDMMwPj?usp=sharing

You can also find the original datasets in the following sources:

- [CICIDS2017](https://www.unb.ca/cic/datasets/ids-2017.html)
- [CICIOT2023](https://www.unb.ca/cic/datasets/iotdataset-2023.html)
- [InSDN Dataset](https://aseados.ucd.ie/datasets/SDN/)


## Models Trained

The project currently includes:

- CNN
- LSTM
- AE-LSTM

Each model is trained using standard preprocessing (scaling, encoding, binary labeling).

---

## Project Structure

The project is organized into three main notebook categories:

### 1. `notebooks/data_processing/`  
Contains notebooks for **preprocessing** raw datasets (handling missing values, scaling, encoding, etc.).  
Run once at the beginning per dataset.  
Processed data is saved to `preprocessed_data/` for reuse.

### 2. `notebooks/model_training/`  
Contains the training scripts for CNN, LSTM, and AE-LSTM models.  
Trained models are saved to the `models/` directory.

### 3. `notebooks/attacks/`  
Implementation of **adversarial attacks** (e.g., HopSkipJump, Boundary Attack) using the **Adversarial Robustness Toolbox (ART)** to evaluate model robustness.

---

## Literature Review

I have written a [literature review](./literature_review_Maxime_BOSSANT.pdf) to summarize the key aspects of this research domain. It covers:
- Threats in SDN-IoT Networks
- Defense Mechanisms and Detection Strategies
- Deep Learning Models for Anomaly Detection

## Literature

The `literature/` folder contains key papers on:
- SDN-specific intrusion detection
- Deep learning models in network security
- Model extraction and adversarial attacks

## Tools & Technologies used

- Python, TensorFlow
- CICIDS2017, InSDN, CICIOT23 datasets
- NumPy, Pandas, Scikit-learn, Foolbox/ART