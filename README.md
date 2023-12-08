# Breast Cancer Metastasis Detection

## Introduction
This repository contains the code and models developed for the private Kaggle competition as part of the deep learning course in the Master's program of Artificial Intelligence. The competition focused on designing deep learning models for the detection of breast cancer metastases in underarm lymph nodes.

## Problem Statement
The task involved predicting whether a given histopathology image of a lymph node section is "normal" (0) or indicates the presence of "cancer" (1). The dataset, consisting of cropped images from histopathology slides, was labeled with these binary classifications.

## Dataset
The dataset used in this competition is based on histopathology slides of lymph node sections, as described in the paper by Bejnordi et al. [1]. The images are labeled as "normal" or "cancer."

## References
[1] Bejnordi, B. E., Veta, M., Van Diest, P. J., Van Ginneken, B., Karssemeijer, N., Litjens, G., … & CAMELYON16 Consortium. (2017). Diagnostic assessment of deep learning algorithms for the detection of lymph node metastases in women with breast cancer. Jama, 318(22), 2199-2210.

## Evaluation Metric
The competition was evaluated using the Area Under Receiver Operating Characteristic Curve (AUROC) as the metric. AUROC is commonly used to assess the diagnostic ability of a binary classifier system as its discrimination threshold is varied. A random guess would produce an AUROC value around 0.5, while a perfect classifier would yield an AUROC value of 1.

## Submission Format
For each image in the dataset, submission files were required to contain two columns: `img_id` and `cancer_score`. The `cancer_score` represents the probability that an image belongs to the cancer class, i.e., the softmax output for the cancer class. Refer to the `sample_submission.csv` for the submission file format.
## Results
After submission and prediction on the test data, the model achieved an AUROC score of 0.84. This indicates a strong performance in distinguishing between normal and cancerous lymph node images.
