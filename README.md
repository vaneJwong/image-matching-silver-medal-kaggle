# Google Image Matching Challenge – Kaggle Silver Medal 🥈

This repository showcases my solution for the  
**Kaggle Google Image Matching Challenge (2022)**,  
where I achieved a **Silver Medal**, ranking **40th out of 642 teams worldwide**.

The competition focuses on registering two images captured from different viewpoints
by identifying reliable correspondences and estimating accurate geometric relationships.

---

## Project Background

With the widespread availability of cameras on mobile devices, massive collections
of unstructured images of landmarks and scenes are generated every day.
Individually, each image provides only a limited two-dimensional view.
However, when combined across many viewpoints, these images can enable
three-dimensional reconstruction of the real world.

This challenge addresses a core problem in computer vision:
**image matching under wide-baseline and real-world conditions**.
It serves as a fundamental building block for
Structure-from-Motion (SfM), which is widely used in applications such as
3D reconstruction, visual localization, and large-scale mapping systems
including Google Maps.

---

## Problem Definition

The task is to estimate the **relative camera pose** between two images taken from
different viewpoints of the same scene.

This is achieved by:
- Detecting **local features** that can be reliably identified across views
- Matching these features between image pairs
- Estimating the **fundamental matrix**, which encodes the epipolar geometry
  between the two camera views

Accurate estimation enables triangulation of corresponding points and
forms the basis for recovering 3D structure.

---

## Approach Overview

My solution emphasizes robustness and geometric consistency under challenging conditions,
including large viewpoint changes, illumination variation, occlusions, and visual clutter.

Key components of the approach include:

- Local feature extraction
- Feature descriptor matching and filtering
- Outlier rejection and geometric verification
- Pose estimation via fundamental matrix prediction

These components are designed to improve matching precision and stability
across diverse real-world scenes.

---

## Evaluation Metric

Submissions are evaluated using **mean Average Accuracy (mAA)**,
which measures the accuracy of the estimated relative pose.

The metric evaluates errors in:
- **Rotation** (in degrees)
- **Translation** (in meters)

Performance is averaged across multiple threshold pairs and scenes,
rewarding solutions that achieve high accuracy under both strict
and relaxed conditions.

---

## Results

- 🏆 **Silver Medal**
- 🌍 Ranked **40 / 642 teams** globally
- Successfully handled wide-baseline image matching scenarios

This result reflects strong performance in both accuracy and robustness
across the competition dataset.


## Repository Structure
```

image-matching-silver-medal-kaggle/
├── notebooks/ # Main experiments and analysis notebooks
├── src/ # Core feature extraction and matching logic
├── results/ # Visualizations and leaderboard screenshots
└── README.md

## How to Navigate This Repository

- Start with the root README for an overview of the project and results
- See `notebooks/` for experimental analysis and exploration
- See `src/` for core implementation of the image matching pipeline
- See `results/` for visualizations and leaderboard screenshots

## Notes

- This repository is intended for **project and portfolio showcase purposes**
- The dataset is provided by Kaggle and is not redistributed here
- The implementation highlights methodology and system design rather than full reproducibility

## Acknowledgments

This competition is organized by Google in collaboration with
the University of British Columbia and Czech Technical University,
and is part of the *Image Matching: Local Features and Beyond*
workshop at **CVPR 2022**.











