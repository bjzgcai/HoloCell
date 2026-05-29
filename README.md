# HoloCell: A Generative Foundation Model for Holistic Cellular Modeling

**HoloCell** is a generative foundation model for holistic single-cell multi-omics modeling across epigenomics, transcriptomics, and proteomics.

HoloCell is designed to learn a unified, holographic representation of cellular states by modeling chromatin accessibility, gene expression, and protein abundance within a shared framework. It supports representation learning, paired and unpaired multi-omics integration, cross-modal alignment, and zero-shot cross-modal generation following the epigenome--transcriptome--proteome axis.

> **Note**
> This repository is currently under active preparation. Source code, pretrained model weights, data processing scripts, tutorials, and benchmark pipelines will be released in a future update.

---

## Overview

Recent advances in single-cell technologies have enabled large-scale profiling of multiple molecular layers within individual cells. However, most existing methods are designed for a single modality, a specific modality pair, or a dataset-specific integration task. HoloCell aims to provide a unified generative foundation model that can jointly represent and generate cellular profiles across major single-cell omics layers.

HoloCell is pretrained on large-scale human single-cell omics data, including unimodal epigenomic, transcriptomic, and proteomic profiles, as well as paired epigenomic--transcriptomic and transcriptomic--proteomic measurements. By combining gene-anchored hierarchical tokenization, Transformer-based representation learning, and diffusion-style masked generation, HoloCell provides a flexible framework for holistic cellular modeling.

---

## Key Features

* **Unified multi-omics modeling**
  HoloCell models epigenomic, transcriptomic, and proteomic profiles within a shared tokenization and representation framework.

* **Gene-anchored hierarchical tokenization**
  cis-regulatory elements, genes, and proteins are represented as structured token triplets, allowing heterogeneous molecular features to be processed by a single model.

* **Large-scale foundation model pretraining**
  HoloCell is pretrained on large-scale single-cell omics data through unimodal and paired multimodal pretraining stages.

* **Single-cell representation learning**
  The model extracts transferable cell embeddings for clustering, visualization, annotation, and downstream analysis.

* **Paired and unpaired multi-omics integration**
  HoloCell supports integration of paired multi-omics profiles and alignment of unpaired modalities through shared cell-state representations.

* **Cross-modal generation**
  HoloCell enables zero-shot generation across molecular layers, including ATAC-to-RNA and RNA-to-protein prediction, using iterative diffusion-style remasking and decoding.

* **Central-dogma-oriented modeling**
  The framework supports generation along the epigenome--transcriptome--proteome axis, providing a foundation for modeling how regulatory states are connected to cellular phenotypes.

---

## Repository Status

This repository currently serves as the official project page for HoloCell. We are organizing the codebase, pretrained checkpoints, data preprocessing workflows, and benchmark scripts for public release.

Planned releases include:

* Model architecture implementation
* Tokenization and preprocessing scripts
* Pretrained HoloCell model weights
* Inference scripts for cell representation extraction
* Scripts for paired and unpaired multi-omics integration
* Cross-modal generation pipelines
* Benchmarking and evaluation code
* Example tutorials and demo datasets
* Documentation for reproducing major results

---

## Citation

If you use HoloCell or refer to this repository, please cite our manuscript.

```bibtex
@article{jiang2026holocell,
  title   = {HoloCell: A Generative Foundation Model for Holistic Cellular Modeling},
  author  = {Jiang, Qun and Li, Zhen and Hu, Bowen and Bie, Yunlong and Li, Keyi and Chen, Xiaoyang and Qin, Tao and Liu, Haiguang and Jiang, Rui and Yin, Qijin},
  journal = {bioRxiv},
  year    = {2026}
}
```

The citation information will be updated after the preprint becomes available online.

---

## License

The license for this repository will be specified before the public release of the source code and model weights.

---

## Contact

For questions or collaboration inquiries, please contact the corresponding authors listed in the manuscript.
