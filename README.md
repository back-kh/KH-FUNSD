# KH-FUNSD: A Hierarchical and Fine-Grained Layout Analysis Dataset for Low-Resource Khmer Business Documents

[![Paper](https://img.shields.io/badge/arXiv-2512.11849-b31b1b.svg)](https://arxiv.org/abs/2512.11849)
[![Status](https://img.shields.io/badge/Status-Under%20Review-yellow)]()
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue)](LICENSE)

## 📋 Overview

**KH-FUNSD** is the first publicly available, hierarchically annotated dataset for Khmer form document understanding. This work addresses a critical gap in document AI tools for low-resource, non-Latin scripts by providing comprehensive resources for analyzing business documents (receipts, invoices, quotations) in Khmer—a language spoken by over 17 million people in Cambodia.

Our annotation framework features a **three-level hierarchical design** that supports both comprehensive layout analysis and precise information extraction, making it valuable for both research and practical applications in document processing.

## 🎯 Key Contributions

- **First Khmer Dataset**: The first publicly available document understanding dataset for Khmer, addressing a major gap in low-resource language processing
- **Three-Level Annotation Framework**: A comprehensive hierarchical annotation scheme that captures multiple levels of document structure and semantics
- **Business Document Focus**: Specialized dataset for practical business documents (receipts, invoices, quotations) critical for administration and enterprise
- **Baseline Results**: First benchmark results for Khmer business documents using leading layout analysis models
- **Insights for Non-Latin Scripts**: Analysis of unique challenges posed by non-Latin, low-resource script document understanding

## 🔍 Research Motivation

Document layout analysis is crucial for automated document processing, information extraction, and digital transformation. However, existing datasets and tools are heavily biased toward Latin scripts and well-resourced languages. Khmer script presents distinct challenges:

- **Low-resource context**: Limited annotated data and computational resources
- **Non-Latin characteristics**: Unique script properties and layout patterns
- **Business document complexity**: Form structures with intricate relationships between fields and values
- **Regional importance**: Critical for Cambodia's public administration and enterprise operations

KH-FUNSD addresses these challenges with tailored resources and analysis.

## 📊 Dataset Description

### Three-Level Annotation Framework

| Level | Component | Description |
|-------|-----------|-------------|
| **Level 1** | Region Detection | Document zone segmentation (header, form fields, footer, body) |
| **Level 2** | FUNSD-style Annotation | Entity classification (questions, answers, headers, other) + relationships |
| **Level 3** | Fine-grained Classification | Semantic role assignment (field labels, values, headers, footers, symbols) |

### Document Types

| Type | Description | Count |
|------|-------------|-------|
| **Receipts** | Point-of-sale and transaction records | - |
| **Invoices** | Commercial billing documents | - |
| **Quotations** | Price estimates and proposals | - |

### Dataset Statistics

- **Scripts**: Khmer (non-Latin)
- **Language**: Khmer
- **Document Types**: 3 (receipts, invoices, quotations)
- **Annotation Levels**: 3 (hierarchical)
- **Availability**: Under journal review – will be released upon publication

## 🔗 Dataset Access

> ⚠️ **Status**: The dataset is currently **under journal review** for APSIPA ASC 2025. Full dataset and documentation will be made publicly available upon publication.

**Planned Release Channels**:
- 📦 GitHub Repository (this repository)
- 🤗 Hugging Face Datasets
- 📋 Official Dataset Portal (to be announced)

*Check back soon for dataset availability links*

## 📈 Methodology

### Baseline Models

We benchmark several leading layout analysis models on KH-FUNSD:

- **YOLOv8-based Region Detection**: For document zone segmentation
- **Faster R-CNN**: For entity detection and localization
- **Transformer-based Methods**: For semantic role classification
- **Graph Neural Networks**: For relation extraction between form elements

### Evaluation Metrics

- **Region Detection**: mAP (mean Average Precision)
- **Entity Detection**: Precision, Recall, F1-score
- **Semantic Classification**: Macro/Micro F1-scores
- **Relation Extraction**: Entity pair accuracy

## 🔬 Key Findings

- Baseline models show promising but distinct performance patterns on non-Latin scripts
- Fine-grained hierarchical annotation enables precise information extraction
- Khmer business documents present unique challenges compared to Latin-script datasets
- Transfer learning from related scripts shows potential but requires careful adaptation

## 💻 Usage

### Installation

```bash
# Clone the repository
git clone https://github.com/back-kh/KH-FUNSD.git
cd KH-FUNSD

# Install dependencies
pip install -r requirements.txt
```

### Loading the Dataset

```python
# Example: Load and explore the dataset (available upon publication)
from datasets import load_dataset

# Dataset will be available at:
# dataset = load_dataset("KH-FUNSD")

# Access document samples
# train_samples = dataset['train']
# for sample in train_samples:
#     print(sample['document_id'])
#     print(sample['regions'])  # Level 1 annotations
#     print(sample['entities'])  # Level 2 annotations
#     print(sample['semantic_roles'])  # Level 3 annotations
```

### Running Baseline Models

```python
# Example: Run region detection baseline (available upon publication)
# from models import RegionDetectionModel
# 
# model = RegionDetectionModel.from_pretrained('kh-funsd-yolov8')
# predictions = model.predict('path/to/document.jpg')
# 
# # Process results
# for region in predictions:
#     print(f"Region type: {region['type']}")
#     print(f"Confidence: {region['confidence']}")
```

## 📝 Citation

If you use KH-FUNSD in your research, please cite:

```bibtex
@article{thuon2025khfunsd,
  title={KH-FUNSD: A Hierarchical and Fine-Grained Layout Analysis Dataset for Low-Resource Khmer Business Documents},
  author={Thuon, Nimol and Du, Jun},
  journal={arXiv preprint arXiv:2512.11849},
  year={2025}
}
```

## 📚 Related Work

### Document Understanding Datasets
- **FUNSD**: Form Understanding in Noisy Scanned Documents
- **RVL-CDIP**: Tobacco-800 and similar document classification datasets
- **DocVQA, InfographicsVQA**: Document-based question answering

### Low-Resource Script Research
- **Indic NLP**: Resources for Indian scripts
- **Thai Document Processing**: Southeast Asian language datasets
- **Arabic/Farsi Document Analysis**: Non-Latin script studies

### Form Document Analysis
- **LayoutLM, LayoutLMv2, LayoutLMv3**: Vision-language models for document understanding
- **Hierarchical Document Models**: Multi-level annotation approaches

## 🤝 Contributing

We welcome contributions! Please feel free to:
- Report issues and bugs
- Suggest improvements to the annotation framework
- Propose baseline model implementations
- Share analysis insights

*Note: Dataset contributions will be accepted after publication.*

## 📧 Contact

For questions, feedback, or collaboration inquiries:

- **Nimol Thuon**: [Contact]
- **Jun Du**: [Contact]
- **GitHub Issues**: [Report issues here](https://github.com/back-kh/KH-FUNSD/issues)

## ⚖️ License

- **Code**: MIT License
- **Dataset**: CC BY-NC 4.0 (upon release)

*This work is currently under review for APSIPA ASC 2025. The dataset and full documentation will be made publicly available upon publication.*

## 🔔 Updates

- **2025-07-11**: Repository created, under review
- **Coming Soon**: Dataset release upon journal publication
- **Coming Soon**: Baseline model implementations
- **Coming Soon**: Detailed annotation guidelines
- **Coming Soon**: Extended analysis and ablation studies

---

**Last Updated**: May 2026

For the latest updates, please watch this repository ⭐
