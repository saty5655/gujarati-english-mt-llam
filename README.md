# gujarati-english-mt-llama

Efficient Few-Shot Gujarati-to-English Machine Translation using Quantized LLaMA Models and LoRA Fine-Tuning | ICICAT 2025

## 📌 Overview
This repository contains the implementation of an efficient Gujarati-to-English machine translation system using quantized LLaMA 3.1 models with LoRA-based fine-tuning. The project addresses the challenge of low-resource machine translation by combining quantization, parameter-efficient fine-tuning (LoRA), and few-shot learning to achieve competitive performance with minimal computational resources.

## 🏆 Key Results

| Metric | Zero-Shot | 3-Shot |
|--------|-----------|--------|
| BLEU Score | 3.43 | 13.77 |
| chrF Score | 8.53 | 39.29 |
| METEOR Score | 17.45 | 40.10 |
| ROUGE-L | 14.01 | 38.17 |
| TER (↓) | 115.39 | 90.16 |

## 🧠 Methodology
- **Base Model:** Meta LLaMA 3.1 (3B / 8B parameters)
- **Quantization:** 4-bit / 8-bit precision to reduce memory footprint
- **Fine-Tuning:** LoRA (Low-Rank Adaptation) — updates only a small subset of parameters
- **Learning Strategy:** Few-shot learning (3-shot) to handle limited Gujarati-English parallel data
- **Framework:** PyTorch + Hugging Face Transformers


##  Dataset

The dataset consists of **Gujarati-English parallel sentence pairs**, sourced from publicly available corpora:

### Sources
| Source | Description | Link |
|--------|-------------|------|
| **AI4Bharat** | Multilingual corpora for Indic languages | [arXiv:2009.06354](https://arxiv.org/abs/2009.06354) |
| **OPUS Corpus** | Open parallel corpora for machine translation | [opus.nlpl.eu](https://opus.nlpl.eu) |
| **Indic NLP Library** | NLP tools and resources for Indian languages | [GitHub](https://github.com/anoopkunchukuttan/indic_nlp_library) |



