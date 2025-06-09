# Data-Free Adversarial Attacks on DL Models in SDN-IoT Networks

This project explores **data-free adversarial attacks** on **Deep learning-based Autonomous anomaly detection** in **SDN** (Software Defined Network)-**IoT**(Internet of Things) networks. We analyse their impact on **CNN**, **LSTM**, and **AE-LSTM** models using **CICIDS2017**, **InSDN**, and **CICIOT23** datasets.

## Datasets Used

Datasets are **not included** in this repo due to size. Please download them manually from the following sources:

- [CICIDS2017](https://www.unb.ca/cic/datasets/ids-2017.html)
- [CICIOT2023](https://www.unb.ca/cic/datasets/iotdataset-2023.html)
- [InSDN Dataset](https://aseados.ucd.ie/datasets/SDN/)


## Models Trained

The project currently includes:

- CNN-based IDS
- LSTM-based IDS
- AE-LSTM

Each model is trained using standard preprocessing (scaling, encoding, binary labeling).


## Literature Review

I have written a literature review (`literature_review_Maxime_BOSSANT.pdf`) to summarize the key aspects of this research domain. It covers:
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