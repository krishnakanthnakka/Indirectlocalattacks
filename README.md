# Indirect Local Attacks for Context-aware Semantic Segmentation Networks 

### Introduction

This repository is a PyTorch implementation of indirect local attacks for semantic segmentation paper(https://arxiv.org/abs/1911.13038)  accepted at ECCV 2020. The code is easy to use for attacking various datasets. The codebase mainly uses ResNet50 as backbone and can be easily adapted to other basic classification structures. 

<img src="./teaser.png" width="900"/>

### Usage

1. Download the Cityscapes sampled  demo images and pretrained public models

     ```
     cd pretrained/
     bash download_dataset.sh
     bash download_pretrained_models.sh
     ```
     
2. Adaptive attack a sample image on a pretrained model with  a given sparsity level 

     ```shell
     sh scripts/adaptive_attack.sh cityscapes psanet50 1.jpg 0.75
     ```

### Citation

If you find the code  useful, please consider citing:

```
@misc{indirectattacks2020,
  author={Krishna Kanth Nakka, Mathieu Salzmann},
  title={indirectattacks},
  howpublished={\url{https://arxiv.org/abs/1911.13038?utm_source=feedburner&utm_medium=feed&utm_campaign=Feed%3A+arxiv%2FQSXk+%28ExcitingAds%21+cs+updates+on+arXiv.org%29}},
  year={2020}
}
