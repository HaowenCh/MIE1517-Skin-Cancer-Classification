# MIE1517 Skin Cancer Classification

**MIE1517 Course Project — Team 1**

## Team Members

| Name | Student ID |
|------|------------|
| Haowen Chang | 1006205394 |
| Purui Yi | 1005789737 |
| Yushu Ding | 1005841840 |

## Project Description

This project develops an automated skin cancer detection system using 3D Total Body Photography (TBP) images combined with clinical metadata.

The core approach employs a **hybrid deep learning architecture** that integrates:
- **DenseNet** — for fine-grained texture feature extraction
- **EfficientNet** — for efficient multi-scale pattern recognition

Both CNNs process lesion images in parallel, leveraging their complementary strengths. Their extracted features are then fused alongside patient metadata before final classification, maximizing diagnostic accuracy.

## Motivation

Skin cancer is one of the most common types of cancer, with current clinical diagnostic accuracy around 70–80%. The visible medical signs of skin cancers follow several specific patterns on the skin that are well-suited for deep learning-based recognition.

This project applies CNN-based models trained from our own methodology, without directly replicating prior work, to develop and fine-tune a model that can reliably identify skin cancer types from images.

## Datasets

### Training Dataset — SLICE-3D
- Source: [ISIC 2024 Challenge](https://challenge2024.isic-archive.com/)
- ~401,059 samples

### Test Dataset — HAM10000
- Source: [Kaggle — Skin Cancer MNIST: HAM10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000)
- ~10,015 samples
- Requires initial data engineering to match the resolution of the SLICE-3D dataset and to address sample bias
