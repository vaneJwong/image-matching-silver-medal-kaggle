# Source Code

This folder contains the core implementation of the image matching pipeline,
including feature extraction, descriptor matching, and geometric verification.

The code focuses on robustness under wide baseline and real world conditions.
## Code Structure

Planned / representative modules:

- `feature_extraction.py`  
  Feature detection and descriptor extraction (e.g. keypoints, descriptors)

- `matching.py`  
  Descriptor matching and filtering

- `geometry.py`  
  Geometric verification and pose estimation

- `pipeline.py`  
  End-to-end image matching pipeline
