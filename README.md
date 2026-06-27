# SemLoD-GS

This repository provides partial implementation materials and supplementary visualization results for the paper:

**SemLoD-GS: Semantic Guidance for Level of Detail Gaussian Splatting in Large-scale Scene Reconstruction**

## Overview

SemLoD-GS is a semantic-aware hierarchical 3D Gaussian Splatting method for large-scale scene reconstruction. It organizes local Gaussian primitives with semantic structure anchors, performs semantic-aware Level-of-Detail (LOD) scheduling, and introduces cross-view temporal consistency optimization to improve rendering stability during large-scale scene roaming.

The complete training and evaluation code will be released upon acceptance.

## Framework

The overall framework of SemLoD-GS is shown below. The method first constructs semantic structure anchors from SfM point clouds and multi-view image features, then performs semantic-aware LOD scheduling and temporal consistency optimization for efficient and stable rendering.

![Overall framework](framework.png)

## Qualitative Results on the Large-scale Dataset

The following figure shows qualitative comparison results on the Large-scale dataset. SemLoD-GS preserves more structural details in large-scale scenes, including building contours, road boundaries, parking areas, and distant structures.

![Qualitative comparison on the Large-scale dataset](qualitative_large.png)

## Gaussian Primitive Visualization

The following visualization shows rendered 2D images together with the corresponding Gaussian primitives. SemLoD-GS preserves fine background details with high visual quality while maintaining real-time rendering performance.

![Gaussian primitive visualization](gaussian_primitives.png)

## Temporal Stability Visualization

The following figure shows temporal stability visualization across consecutive views. By introducing temporal consistency optimization, SemLoD-GS reduces flickering and level popping during continuous scene roaming.

![Temporal stability visualization](temporal_stability.png)

## Repository Status

The current version includes:

* Partial implementation materials
* Visualization results
* Supplementary figures
* Example configuration and running instructions to be updated

The full source code, training scripts, evaluation scripts, and detailed documentation will be made publicly available after acceptance.

## Citation

If you find this work useful, please consider citing our paper:

```bibtex
@article{chen2026semlodgs,
  title={SemLoD-GS: Semantic Guidance for Level of Detail Gaussian Splatting in Large-scale Scene Reconstruction},
  author={Chen, Wentao and Zou, Yaqi and Chen, Zhong and Wang, Fahou and Li, Hui},
  journal={IEEE Transactions on Visualization and Computer Graphics},
  year={2026}
}
```
