# AI Challenge - Prediction of Spatial Cellular Organization from Histology Images

## Problem Statement
Map the spatial distribution of biological cell types in a tissue slice from routine Histology HE slides.

## Introduction & Background
Histology is a century-old technique critical for clinical diagnosis. However, its interpretation is subjective, time-consuming, and limited to coarse-grained features. In contrast, genomic deep sequencing and spatial transcriptomics provide rich molecular details but are cost-prohibitive and technically demanding.

This challenge invites participants to bridge this gap by predicting cell-type composition directly from HE images, leveraging machine learning to infer spatial patterns of biological signals from routine data.

## Core Challenge
Design a computational pipeline to predict the spatially resolved cell-type composition of a tissue sample. For each spot (~55 μm in diameter), the goal is to predict the abundances of **35 cell types** using image data alone.

## Submission Requirements
- Notebook submissions with run-time ≤ 9 hours (CPU or GPU).
- No external data – only the provided training set and public models/libraries.
- The submission file must be named `submission.csv` and follow the format:
  `ID,C1,C2,...,C35`
  where C1-C35 are the predicted cell-type abundances on the test slide 'S_7'.

## Evaluation
Submissions will be scored by the **Spearman correlation** between predicted and ground truth cell-type abundances.