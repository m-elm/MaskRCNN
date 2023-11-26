# Spherocytosis MaskRCNN Detection

An AI-powered tool for the early detection of Hereditary Spherocytosis and related blood disorders using Mask R-CNN in TensorFlow.

## Table of Contents

1. [What is Hereditary Spherocytosis (HS)?](#1-what-is-hereditary-spherocytosis)
2. [What does the MaskRCNN Model Detect?](#2-what-does-the-maskrcnn-model-detect)
3. [Data](#3-data)
4. [Bibliography](#4-bibliography)
5. [The Model](#5-the-model)

## 1. What is Hereditary Spherocytosis (HS)? 💉 🩸

According to [Nemours KidsHealth](https://kidshealth.org/en/parents/hereditary-spherocytosis.html), Hereditary Spherocytosis (HS) is an inherited blood disorder characterized by spherical-shaped red blood cells (spherocytes) that are more fragile than normal disc-shaped cells. This condition leads to [hemolytic anemia](https://kidshealth.org/en/parents/anemia-hemolytic.html) and other health complications. Symptoms can range from mild to severe, with available treatments to manage them.

![Hereditary Spherocytosis](https://assets.aboutkidshealth.ca/akhassets/hereditary_spherocytosis_EN.png)

## 2. What does the MaskRCNN Model Detect? 🚀🚀

The Mask R-CNN model, trained on a dataset of digital images of MGG-stained blood smears, can efficiently detect Hereditary Spherocytosis. Traditionally, identifying spherocytes in blood smears is a time-consuming process performed by pathologists. The MaskRCNN model automates this process, offering a quicker and more accessible solution for both patients and physicians.

## 3. Data

* [Dataset A: 186 digital images of MGG-stained blood smears from five patients with hereditary spherocytosis](https://data.mendeley.com/datasets/c37wnbbd3c/1): This dataset comprises high-resolution images acquired through a microscope with 1,000x magnification (Olympus BX43) and a digital camera (Olympus DP73). The images are in JPG format (RGB, 2,400 x 1,800 pixels).

## 4. Bibliography

* Delgado-Ortet M, Molina A, Alférez S, Rodellar J, Merino A. [A Deep Learning Approach for Segmentation of Red Blood Cell Images and Malaria Detection](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7517192/). Entropy (Basel). 2020 Jun 13;22(6):657. PMID: 33286429; PMCID: PMC7517192.
* Naruenatthanaset K., Chalidabhongse T. H., Palasuwan D., Anantrasirichai N., Palasuwan A.. [Red Blood Cell Segmentation with Overlapping Cell Separation and Classification on Imbalanced Dataset](https://arxiv.org/abs/2012.01321). 2023. arXiv:2012.01321.
* Sadafi A., Bordukova M., Makhro A., Navab N., Bogdanova A., Marr C. [RedTell: an AI tool for interpretable analysis of red blood cell morphology](https://www.frontiersin.org/articles/10.3389/fphys.2023.1058720). Frontiers in Physiology Vol 14 (2023). DOI=10.3389/fphys.2023.1058720. ISSN=1664-042X.

## 5. The Model

The model utilized is Mask R-CNN with Mobilenet V2 as the backbone model from the TensorFlow Model Garden. The dataset was labeled using Roboflow.

---
