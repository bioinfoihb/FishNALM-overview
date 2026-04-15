# FishNALM

**FishNALM: A Fish-Specific Foundation DNA Language Model for Fish Genomes**

## Overview

FishNALM is a fish-specific foundation DNA language model framework designed for fish genomes. It aims to learn biologically meaningful sequence representations from large-scale fish genomic sequences and support downstream genomic analyses, including promoter prediction, transcription factor binding-site prediction, histone-mark prediction, splice-site prediction, and variant-effect analysis.

The FishNALM family currently includes four pretrained models built from two data scales and two model scales:

- **FishNALM-8** and **FishNALM-8L**: pretrained on 8 core cyprinid fish genomes  
- **FishNALM-20** and **FishNALM-20L**: pretrained on 20 diverse fish genomes  

FishNALM adopts a **BERT-style encoder-only Transformer** and is pretrained with **masked language modeling (MLM)**. The tokenizer uses a **6-mer + BPE** hybrid strategy.

---

## Code availability

The FishNALM code repository has been established at:

**GitHub:** https://github.com/bioinfoihb/FishNALM

To avoid affecting the peer-review and publication process, the source code is **currently kept private**.  
The **full codebase will be released publicly upon publication** of the corresponding paper.

At the current stage, this repository is intended to provide project information and access points for released models and datasets. More complete documentation and runnable code will be made available after publication.

---

## Pretrained models

Pretrained FishNALM models are available at Hugging Face:

**Hugging Face organization:** https://huggingface.co/bioinfoihb

- **FishNALM-8**  
  https://huggingface.co/bioinfoihb/FishNALM-8_pretrain

- **FishNALM-8L**  
  https://huggingface.co/bioinfoihb/FishNALM-8L_pretrain

- **FishNALM-20**  
  https://huggingface.co/bioinfoihb/FishNALM-20_pretrain

- **FishNALM-20L**  
  https://huggingface.co/bioinfoihb/FishNALM-20L_pretrain

---

## Datasets

The FishNALM-related datasets are available at Hugging Face:

- **Fish_GUE**  
  https://huggingface.co/datasets/bioinfoihb/Fish_GUE

- **FishNALM-8 pretrain corpus**  
  https://huggingface.co/datasets/bioinfoihb/FishNALM-8-pretrain-corpus

- **FishNALM-20 pretrain corpus**  
  https://huggingface.co/datasets/bioinfoihb/FishNALM-20-pretrain-corpus

---

## Model summary

| Model | Pretraining data | Approx. parameters | Architecture |
| --- | --- | ---: | --- |
| FishNALM-8 | 8 fish genomes | ~90M | BERT-style encoder |
| FishNALM-8L | 8 fish genomes | ~310M | BERT-style encoder |
| FishNALM-20 | 20 fish genomes | ~90M | BERT-style encoder |
| FishNALM-20L | 20 fish genomes | ~310M | BERT-style encoder |

Common settings:

- **Tokenization:** 6-mer + BPE  
- **Vocabulary size:** 4863  
- **Maximum input length:** 512 tokens  
- **Pretraining objective:** masked language modeling (MLM)  

---

## Environment

A standard Python environment with PyTorch and common deep-learning dependencies is recommended.

Example:

```bash
conda create -n fishnalm python=3.11
conda activate fishnalm
pip install -r requirements.txt
```

For GPU usage, please install the PyTorch version appropriate for your CUDA environment.

Detailed environment configuration and complete running instructions will be provided together with the public code release after publication.

---

## Usage

FishNALM is designed to support three major usage scenarios:

- **Pretraining**
- **Fine-tuning on downstream genomic tasks**
- **Inference with trained models**

At present, only a brief project description is provided here.  
Detailed scripts, examples, and runnable workflows will be released after publication.

---

## Applications

FishNALM is developed for fish genomic sequence modeling and can be applied to tasks such as:

- promoter prediction
- transcription factor binding-site prediction
- histone-mark prediction
- splice-site prediction
- zero-shot variant-effect analysis

---

## Paper

**FishNALM: A Fish-Specific Foundation DNA Language Model for Fish Genomes**

---

## License

License information for the code release will be provided upon publication.

---

## Contact

**Xiao-Qin Xia**  
Institute of Hydrobiology, Chinese Academy of Sciences  

Email: xqxia@ihb.ac.cn  
Email: bioinfoihb@ihb.ac.cn
