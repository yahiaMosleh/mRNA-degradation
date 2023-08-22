# mRNA-degradation
mRNA Vaccine Degradation Prediction
This project focuses on predicting degradation-prone segments within mRNA vaccine sequences for COVID-19 using sequence modeling techniques. The goal is to provide insights into areas of vulnerability in order to address degradation challenges associated with mRNA vaccines.

Table of Contents
Introduction
Methods
Results
Usage
Future Work


Introduction
mRNA vaccines have demonstrated remarkable efficacy in combating COVID-19. However, concerns regarding degradation of mRNA sequences have emerged. This project explores the prediction of degradation-sensitive regions in mRNA vaccine sequences. The study involves employing various sequence models to forecast degradation likelihoods.

Methods
Sequence modeling: We utilized multiple sequence models to predict degradation by estimating sets of three reactivity values for each position within the mRNA sequence.
Encoding methods: Two encoding methods, namely label encoding and mapping encoding, were employed to preprocess the sequence data.
Feature importance: We determined feature importance using the "weight" algorithm from the XGBoost library. This helped identify positions in the sequence consistently used for degradation predictions.
Results
The mapping encoding method outperformed others, achieving a 0.33 score through weighted MCRMSE averaging. However, overfitting concerns were observed in training/validation losses, indicating the need for careful model selection and regularization.

Usage
Clone the repository.
Install the required dependencies mentioned in requirements.txt.
Run the provided scripts for data preprocessing, model training, and evaluation.
Future Work
A suggested avenue for future work involves creating a hybrid model by combining convolutional neural networks (CNNs) with sequence models. Furthermore, incorporating graph convolutional networks (GCNs) could lead to improved predictions by leveraging graph-like structures in the sequence data.

Contributing
Contributions to this project are welcome. If you find any issues or have suggestions, please feel free to create a pull request or open an issue.
