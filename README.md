# CoVLM: Leveraging Consensus from Vision-Language Models for Semi-supervised multi-modal Fake News Detection

## Overview
**CoVLM** addresses the detection of out-of-context misinformation, specifically where a real image is paired with an incorrect caption to create fake news. Our framework leverages a semi-supervised approach, using both limited labeled data and a large corpus of unlabeled data to detect misinformation effectively, even in highly imbalanced datasets.

![Intro Image]([path_to_intro_image.png](https://github.com/devank3/CoVLM/blob/main/Figure/Figure1.pdf))

## Key Features
- **Semi-supervised learning**: Efficiently handles scenarios with limited labeled data and a large amount of unlabeled image-text pairs.
- **Pseudo-label generation**: CoVLM dynamically generates robust pseudo-labels using thresholds derived from the labeled data.
- **Class imbalance handling**: Tackles the issue of imbalanced datasets, where fake news is much less frequent compared to real news.
- **State-of-the-art performance**: CoVLM demonstrates superior results across benchmark datasets, outperforming several existing approaches.

![Feature Diagram](path_to_feature_diagram.png)

## Model Architecture
CoVLM utilizes Vision-Language Models (e.g., CLIP, BLIP) to assess image-caption pairings. A key aspect is the generation of pseudo-labels based on dynamic thresholding, ensuring only confident predictions from the unlabeled set are used for training.

![Model Architecture](path_to_model_architecture_image.png)

## Datasets
The framework is tested on several benchmark datasets for fake news detection:
1. **NewsCLIPpings**
2. **GossipCop**
3. **PolitiFact**

These datasets offer challenging real-world scenarios with imbalanced data distributions.

![Dataset Example](path_to_dataset_example_image.png)

## Installation
Clone the repository and install the required dependencies:

```bash
git clone https://github.com/devank3/CoVLM.git
cd CoVLM
pip install -r requirements.txt
