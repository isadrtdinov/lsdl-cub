# CUB Large Scale Deep Learning Models, Fall 2024

With the advancement of deep learning, an increasing number of new tasks and datasets have emerged, which can be used to train models. However, while collecting data can be done algorithmically without much effort, annotating it is a very labor-intensive and costly process. This has led to the need for training models on unannotated data. This is how the self-supervised learning paradigm came into being, which will be the focus of this course. Course participants will become familiar with both traditional and the most modern approaches to pretraining on unannotated data and will work with various domains, from images and texts to audio and graphs.

**Instructors:** Alexander Shabalin, Ildus Sadrtdinov, Dmitry Kropotov

**Classes:** on Mondays offline in the classroom EH-4 in time slots 14:15 - 15:30 and 15:45 - 17:00

**Telegram chat for questions and discussion:** [link](https://t.me/+jKSAP9vmxPo3NDFi)

**Practical assignments**: all asssignments are given and checked in the corresponding Teams space. If you don't have access to Teams space, please write directly to one of the instructors or in the course chat.

## Course assessment criteria

Assessment Component 1: written examination, Duration: 60 min, Weight: 50 %

Assessment Component 2: programming assignments, Weight: 50 %

Completion: To pass this module, the examination of each module component must be passed with at least
45%.

## Lectures

| Date | Number | Topic | Materials |
| :---: | :---: | --- | --- |
| 09.09.24  | 01  | Introduction to the course. Large models, large datasets and self-supervised learning. What to do with a pretrained model? Linear probing, Fine-tuning, in-distribution (ID) and out-of-distribution (OOD) performance. CLIP model, Zero-shot and WiSE-FT (robust weights ensemble). |  [Fine-tuning distorts features](https://arxiv.org/pdf/2202.10054), [Comparing pre-training algorithms](https://arxiv.org/pdf/2103.14005), [CLIP](https://arxiv.org/pdf/2103.00020), [WiSE-FT](https://arxiv.org/pdf/2109.01903), [Do ImageNet Classifiers Generalize to ImageNet?](https://arxiv.org/pdf/1902.10811)  |
| 23.09.24  | 02  | Classical pretext tasks for images: inpainting, colorization, jigsaw puzzles   |  [Exemplar](https://arxiv.org/abs/1406.6909), [Context Prediction](https://arxiv.org/abs/1505.05192), [Inpainting](https://arxiv.org/abs/1604.07379), [Jigsaw Puzzles](https://arxiv.org/abs/1603.09246), [Colorization](https://arxiv.org/abs/1603.08511), [Rotations](https://arxiv.org/abs/1803.07728), [Damaged Jigsaw Puzzles](https://arxiv.org/abs/1802.01880), [Task Ensemble](https://arxiv.org/abs/1708.07860) |
| 30.09.24  | 03  | Modern architectures for images: ViT, DeiT, MLP Mixer, Swin, ConvNeXt, Neighborhood Attention Transformer (NAT). <br> Efficient training & inference: Automatic Mixed Precision (AMP), Data-Parallel and Model-Parallel training | [Big Transfer](https://arxiv.org/pdf/1912.11370), [ViT](https://arxiv.org/abs/2010.11929), [DeiT](https://arxiv.org/abs/2012.12877), [MLP Mixer](https://arxiv.org/pdf/2105.01601), [Swin](https://arxiv.org/pdf/2103.14030), [ConvNeXt](https://arxiv.org/abs/2201.03545), [NAT](https://arxiv.org/abs/2204.07143) |
| 07.10.24  | 04  | Contrastive learning for images. Mutual information, SimCLR, MoCo, BYOL, SimSiam, DeepCluster, SwAV. Deriving contrastive loss | [SimCLR](https://arxiv.org/pdf/2002.05709.pdf), [MoCo](https://arxiv.org/pdf/1911.05722.pdf), [BYOL](https://arxiv.org/pdf/2006.07733.pdf), [SimSiam](https://arxiv.org/pdf/2011.10566.pdf), [DeepCluster](https://arxiv.org/pdf/1807.05520.pdf), [SwAV](https://arxiv.org/pdf/2006.09882.pdf) |
| 14.10.24  | 05  | Self-supervised learning for ViT. Masked image modeling. DINO, BEiT, MAE, MaskFeat. Different approaches for improving contrastive learning.  | [DINO](https://arxiv.org/pdf/2104.14294.pdf), [BEiT](https://arxiv.org/pdf/2106.08254.pdf), [MAE](https://arxiv.org/pdf/2111.06377.pdf), [MaskFeat](https://openaccess.thecvf.com/content/CVPR2022/papers/Wei_Masked_Feature_Prediction_for_Self-Supervised_Visual_Pre-Training_CVPR_2022_paper.pdf) <br> [Dense CL](https://arxiv.org/pdf/2011.09157.pdf), [Supervised CL](https://arxiv.org/pdf/2004.11362.pdf), [DiLo](https://arxiv.org/pdf/2004.06638.pdf), [LooC](https://arxiv.org/pdf/2008.05659.pdf) | 
| 21.10.24  | 06  | Ensembling & weight averaging. Deep Ensemble, FGE, SSE, SWAG, SPRO, StarSSE, SWA, model soups |  |
| 28.10.24  | 07  | Pruning, Quantization, Distillation |  |
| 04.11.24  | 08  | Modern architectures for texts. Recap of transformers. Modern architectures. Transformer training tricks. What LLMs learn? |  |
| 11.11.24  | 09  | Parameter-Efficient Fine-tuning. GPT zero-shot, Prompt Tuning, Adapters, LoRA, QLoRA |  |
| 18.11.24  | 10  | Retrieval Augmented Generation |  |
| 25.11.24  | 11  | Reinforcement Learning with Human Feedback |  |
| 02.12.24  | 12  | Self-supervised learning for audio. Introduction to audio processing. CPC, Wav2Vec 2.0, HUBERT, Multi-format contrastive learning, BYOL-A. |  |
| 07.12.24  | 13  | Self-supervised learning for graphs. Intro to representation learning on graphs. Review of approaches. |  |

## Home assignments

| Number | Release date | Deadline | Topic |
| :---: | :---: | :---: | :---: |
| 01 | 15.09.24 | 01.10.24 23:59 | [Robust fine-tuning of CLIP](https://github.com/isadrtdinov/lsdl-cub/blob/main/week01-finetune/homework/homework-week01.ipynb) |
| 02 | 01.10.24 | 18.10.24 23:59 | [Classical pre-text tasks](https://github.com/isadrtdinov/lsdl-cub/blob/main/week02-pretext/homework.md) |

## Recommended reading
Some list of materials here
