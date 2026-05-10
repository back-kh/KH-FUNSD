# KH-FUNSD: A Hierarchical and Fine-Grained Layout Analysis Dataset for Low-Resource Khmer Business Documents

[![Paper](https://img.shields.io/badge/arXiv-2512.11849-b31b1b.svg)](https://arxiv.org/abs/2512.11849)
[![Status](https://img.shields.io/badge/Status-Under%20Review-yellow)]()
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-blue)](LICENSE)

## 📋 Overview

**KH-FUNSD** is the first publicly available, hierarchically annotated dataset for Khmer form document understanding. This work addresses a critical gap in document AI tools for low-resource, non-Latin scripts by providing comprehensive resources for analyzing business documents (receipts, invoices, quotations) in Khmer—a language spoken by over 17 million people in Cambodia.

Our annotation framework features a **three-level hierarchical design** that supports both comprehensive layout analysis and precise information extraction, making it valuable for both research and practical applications in document processing.


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

> ⚠️ **Status**: The dataset is currently **under journal review** . Full dataset and documentation will be made publicly available upon publication.


*Note: Dataset contributions will be accepted after publication.*

## 📧 Contact

For questions, feedback, or collaboration inquiries:

- **Nimol Thuon**: nimol.thuon@gmail.com
- **GitHub Issues**: [Report issues here](https://github.com/back-kh/KH-FUNSD/issues)

## 🔔 Updates

- **2025-07-11**: Repository created, under review
- **Coming Soon**: Dataset release upon journal publication
- **Coming Soon**: Extended analysis and ablation studies


## 📝 Citation

If you use KH-FUNSD in your research, please cite:

```bibtex
@inproceedings{thuon2025kh,
  title={KH-FUNSD: A Hierarchical and Fine-Grained Layout Analysis Dataset for Low-Resource Khmer Business Document},
  author={Thuon, Nimol and Du, Jun},
  booktitle={2025 Asia Pacific Signal and Information Processing Association Annual Summit and Conference (APSIPA ASC)},
  pages={1886--1891},
  year={2025},
  organization={IEEE}
}
```

---
