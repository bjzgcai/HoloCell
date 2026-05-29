# HoloCell: A Generative Foundation Model for Holistic Cellular Modeling

**HoloCell** is a generative foundation model for holistic single-cell multi-omics modeling across epigenomics, transcriptomics, and proteomics.

HoloCell is designed to learn a unified, holographic representation of cellular states by modeling chromatin accessibility, gene expression, and protein abundance within a shared framework. It supports representation learning, paired and unpaired multi-omics integration, cross-modal alignment, and zero-shot cross-modal generation following the epigenome--transcriptome--proteome axis.

> **Note**
> This repository is currently under active preparation. Source code, pretrained model weights, data processing scripts, tutorials, and benchmark pipelines will be released in a future update.

---

## Overview

Recent advances in single-cell multi-omics technologies have enabled the profiling of epigenomic, transcriptomic, and proteomic layers within individual cells, providing new opportunities to characterize cellular states as integrated molecular systems. However, learning transferable representations and performing generative modeling across heterogeneous modalities remain challenging. Existing methods are often designed for specific modalities or modality pairs, rely on dataset-specific training or paired measurements, and may impose unnecessary sequential assumptions on unordered molecular profiles. 

Here, we present HoloCell, to our knowledge the first generative foundation model for joint representation learning and generative modeling across all three major single-cell omics modalities—epigenomics, transcriptomics, and proteomics. HoloCell contains over 860 million parameters and is pretrained on the Human-Multi-Omics-Corpus-468M, comprising approximately 468 million single-cell profiles across these three layers. It introduces a unified hierarchical tokenization strategy that encodes cis-regulatory elements, genes, and proteins as structured tokens within a shared modeling framework. 

HoloCell is pretrained through a two-stage paradigm: large-scale unimodal pretraining on 11.4 million epigenomic, 67.9 million transcriptomic, and 383.5 million proteomic profiles, followed by multimodal pretraining on 2.4 million paired epigenomic–transcriptomic cells and 2.9 million paired transcriptomic–proteomic cells. We evaluate HoloCell on single-omics representation learning, paired multi-omics integration, unpaired multi-omics alignment, and cross-modal generation using iterative diffusion and remasking. Across these tasks, HoloCell achieves competitive or improved performance relative to representative baselines, with particular advantages in preserving cell-type-resolved structure and enabling zero-shot cross-modal inference. These results demonstrate that HoloCell serves as a flexible and versatile foundation model, capable of unifying diverse single-cell multi-omics tasks within a single framework.

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
