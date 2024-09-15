# CUB Large Scale Deep Learning Models, Fall 2024

With the advancement of deep learning, an increasing number of new tasks and datasets have emerged, which can be used to train models. However, while collecting data can be done algorithmically without much effort, annotating it is a very labor-intensive and costly process. This has led to the need for training models on unannotated data. This is how the self-supervised learning paradigm came into being, which will be the focus of this course. Course participants will become familiar with both traditional and the most modern approaches to pretraining on unannotated data and will work with various domains, from images and texts to audio and graphs.

**Instructors:** Alexander Shabalin, Ildus Satrdinov, Dmitry Kropotov

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
| 16.09.24  | 02  | Classical pretext tasks for images: inpainting, colorization, jigsaw puzzles   |  |
| 23.09.24  | 03  | Modern architectures for images: ViT, DEiT, Swin, Neighborhood Attention Transformer, MLPMixer, ConvNext |  |
| 30.09.24  | 04  | Contrastive learning for images. Mutual information, SimCLR, MoCo, BYOL, SimSiam, SwAV. Deriving contrastive loss |  |
| 07.10.24  | 05  | Masked image modeling. DINO, BEiT, MAE, MaskFeat. Different approaches for improving contrastive learning.  |  | 
| 14.10.24  | 06  | Ensembling & weight averaging. Deep Ensemble, FGE, SSE, SWAG, SPRO, StarSSE, SWA, model soups |  |
| 21.10.24  | 07  | Pruning, Quantization, Distillation |  |
| 28.10.24  | 08  | Modern architectures for texts. Recap of transformers. Modern architectures. Transformer training tricks. What LLMs learn? |  |
| 04.11.24  | 09  | Parameter-Efficient Fine-tuning. GPT zero-shot, Prompt Tuning, Adapters, LoRA, QLoRA |  |
| 11.11.24  | 10  | Retrieval Augmented Generation |  |
| 18.11.24  | 11  | Reinforcement Learning with Human Feedback |  |
| 25.11.24  | 12  | Self-supervised learning for audio. Introduction to audio processing. CPC, Wav2Vec 2.0, HUBERT, Multi-format contrastive learning, BYOL-A. |  |
| 02.12.24  | 13  | Self-supervised learning for graphs. Intro to representation learning on graphs. Review of approaches. |  |

## Home assignments

| Number | Release date | Deadline | Topic |
| :---: | :---: | :---: | :---: |
| 01 | 15.09.24 | 01.10.24 23:59 | [Robust fine-tuning of CLIP](https://github.com/isadrtdinov/lsdl-cub/blob/main/week01-finetune/homework/homework-week01.ipynb)

## Recommended reading
Some list of materials here
