# CUB Large Scale Deep Learning Models, Fall 2024

The "Large Scale Deep Learning Models" course focuses on the methodologies and techniques used to train large models on extensive datasets across various data domains, including images, text, and audio. The course provides in-depth coverage of self-supervised learning approaches, which have become crucial for leveraging vast amounts of unlabeled data. Topics include data preprocessing and augmentation for different modalities, architectural considerations for scaling deep learning models, and strategies for distributed and parallel training.

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
| 21.10.24  | 06  | Mode connectivity and Linear mode connectivity (LMC). Ensembling: Deep Ensemble (DE), SSE, FGE, cSGLD, KFAC-Laplace, SWAG, SPRO, StarSSE. Model averaging: SWA, model soups. Weight averaging in optimization: Lookahead, Lookaround, WATT | [LMC](https://arxiv.org/pdf/1912.05671), [LMC in transfer learning](https://arxiv.org/pdf/2008.11687), <br> [DE](https://arxiv.org/pdf/1612.01474), [DE and loss landscape](https://arxiv.org/pdf/1912.02757), [DE and distribution shifts](https://arxiv.org/pdf/1906.02530), <br> [SSE](https://arxiv.org/pdf/1704.00109), [FGE](https://arxiv.org/pdf/1802.10026), [cSGLD](https://arxiv.org/pdf/1902.03932), [KFAC-Laplace](https://openreview.net/pdf?id=Skdvd2xAZ), [SWAG](https://arxiv.org/pdf/1902.02476), [SPRO](https://arxiv.org/pdf/2102.13042), [DE Equivalent](https://arxiv.org/pdf/2002.06470), [StarSSE](https://arxiv.org/pdf/2303.03374), <br> [SWA](https://arxiv.org/pdf/1803.05407), [model soups](https://arxiv.org/pdf/2203.05482), [Lookahead](https://arxiv.org/pdf/1907.08610), [Lookaround](https://arxiv.org/pdf/2306.07684), [WATT](https://arxiv.org/pdf/2406.13875) |
| 28.10.24  | 08  | Modern architectures for texts. Recap of transformers. Modern architectures. Transformer training tricks. | [Flash attention](https://arxiv.org/abs/2205.14135), [FA blogpost](https://huggingface.co/docs/text-generation-inference/conceptual/flash_attention), [KV-caching](https://medium.com/@plienhar/llm-inference-series-3-kv-caching-unveiled-048152e461c8), [Multi-Query attention](https://arxiv.org/abs/1911.02150), [Relative Position Encodings](https://arxiv.org/abs/1803.02155), [RoPE](https://arxiv.org/abs/2104.09864), [ALiBi](https://arxiv.org/abs/2108.12409), [GLU](https://arxiv.org/abs/2002.05202), [Mixture of Experts](https://arxiv.org/abs/1701.06538), [Pre-normalization](https://arxiv.org/abs/2002.04745), [RMSNorm](https://arxiv.org/abs/1910.07467) |
| 04.11.24  | 07  | Pruning, Quantization, Distillation | [Pruning](https://proceedings.neurips.cc/paper/1989/hash/6c9882bbac1c7093bd25041881277658-Abstract.html), [Quantization 1](https://huggingface.co/docs/optimum/concept_guides/quantization), [Quantization 2](https://www.tensorops.ai/post/what-are-quantized-llms), [Distillation](https://arxiv.org/abs/1503.02531), [DistilBERT](https://arxiv.org/abs/1910.01108)  |
| 11.11.24  | 09  | Parameter-Efficient Fine-tuning. GPT zero-shot, Prompt Tuning, Adapters, LoRA, BitFit | [GPT-3](https://arxiv.org/abs/2005.14165), [Prompt Tuning](https://arxiv.org/abs/2104.08691), [P-Tuning](https://aclanthology.org/2022.acl-short.8/), [Adapters](https://arxiv.org/abs/1902.00751), [LoRA](https://arxiv.org/abs/2106.09685), [BitFit](https://arxiv.org/abs/2106.10199) |
| 18.11.24  | 10  | Retrieval Augmented Generation |  |
| 25.11.24  | 11  | Reinforcement Learning with Human Feedback |  |
| 02.12.24  | 12  | Self-supervised learning for audio. Introduction to audio processing. CPC, Wav2Vec 2.0, HUBERT, Multi-format contrastive learning, BYOL-A. |  |
| 07.12.24  | 13  | Self-supervised learning for graphs. Intro to representation learning on graphs. Review of approaches. |  |

## Home assignments

| Number | Release date | Deadline | Topic |
| :---: | :---: | :---: | :---: |
| 01 | 15.09.24 | 01.10.24 23:59 | [Robust fine-tuning of CLIP](https://github.com/isadrtdinov/lsdl-cub/blob/main/week01-finetune/homework/homework-week01.ipynb) |
| 02 | 01.10.24 | 18.10.24 23:59 | [Classical pre-text tasks](https://github.com/isadrtdinov/lsdl-cub/blob/main/week02-pretext/homework.md) |
| 03 | 18.10.24 | 06.11.24 23:59 | [Contrastive learning](https://github.com/isadrtdinov/lsdl-cub/blob/main/week04-contrastive/homework/homework-week04.ipynb) |
