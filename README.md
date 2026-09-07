# Project Title: Wildlife Camera Trap Classification

## Problem Definition
In order for conservationists to monitor biodiversity, study inter-species dynamics, and track the impact of climate change, there is an increasing reliance on motion-activated camera traps deployed in the wild. These cameras, triggered by motion, capture millions of images continuously. However, processing this data is a massive bottleneck. Researchers must manually sort through millions of captured pictures to identify which images actually contain animals (as opposed to empty frames triggered by wind or moving vegetation) and further classify the specific species present. This manual analysis is highly time-consuming and resource-intensive, which can delay critical conservation responses. Our team plans to address this bottleneck by automating the detection and classification of wildlife using deep learning.

## Objectives & Goals
The primary goal of this project is to build an automated image classification pipeline with a clear, three-fold prediction objective:

• Binary Classification: The model will first predict whether a given camera trap image contains an animal or is entirely empty (a false trigger).

• Multiclass Classification (Species Identification): For images where an animal is present, the model will classify the specific species of the animal from a predefined set of categories (e.g., lion, zebra, elephant).

• Population Density Estimation (Counting): For images positively identified as containing animals, the model will predict the approximate number of individuals present in the frame (e.g., 1, 2, 3-5, 6+). This extends the pipeline beyond basic species tagging, providing conservationists with automated metrics for herd-size tracking and population density estimation.

## Dataset
We used the Snapshot Serengeti Dataset as proposed. After preprocessing, the final subset consisted of 8312 images across 22 animal species classes, including blank images used for binary classification.
