# Classical-HeLa-Cell-Segmentation
Brief project exploring non-DL/classical image segmentation methods. Principally done via thresholding, morphology, and region-specific geometric analysis

Deterministic, classical computer vision pipeline for segmenting and analysing HeLa cells in fluorescence microscopy images. The algorithm isolates individual cells, fills closed contours to obtain accurate masks, and extracts geometric properties such as cell count, area, centroid, and bounding boxes. Robustness is evaluated under 90 degree rotations.

## Pipeline Overview

### Preprocessing:

Grayscale conversion and intensity normalisation

Background subtraction using a rolling-ball filter

Median filtering for salt-and-pepper noise reduction

Gaussian smoothing for feature stabilisation

### Segmentation:

Adaptive Otsu thresholding

Morphological opening and closing to remove small unwanted structures

Region filling to recover full cell interiors

Exclusion of border-touching objects

### Analysis:

Connected-component labeling

Cell counting

### Displayed geometric region characteristics:

Area

Centroid

Bounding box

Identification and visualisation of the largest detected cell

Robustness Testing

Output consistency is visually and numerically inspected
