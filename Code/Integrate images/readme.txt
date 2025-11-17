---

# BPA Dataset Processing Pipeline

This folder contains the **code and notebooks responsible for generating the final Blood Pattern Analysis (BPA) dataset**. Each script processes a different original dataset, extracts its images, standardizes them, and builds the CSV label files. The outputs from all datasets are then merged into one unified dataset.

---

## 🔧 What the Code Does

The processing pipeline follows these steps for **every original dataset**:

### 1. **Image Extraction**

* Reads all images from the raw dataset.
* Removes invalid or unreadable files.
* Normalizes the file naming format.

### 2. **Image Resizing**

* Each image is resized to **224×224** pixels.
* Ensures all datasets share the same resolution.
* Makes training deep learning models easier on low resources.

### 3. **Label File Generation**

* Creates a CSV file containing:

  * `Image` — the filename only
  * `Class` — the blood pattern category
* Ensures each image is correctly mapped to its label.

### 4. **Data Cleaning**

* Removes duplicates.
* Fixes corrupted images.
* Ensures consistent class naming across datasets.

---

## 🔄 Dataset Integration

After processing each dataset individually, all outputs are **merged and standardized** in the notebook:

### **`gathere.ipynb`**

This notebook performs:

* Combining all individual CSV files
* Merging all processed images into a single directory
* Unifying label structure
* Verifying dataset consistency
* Exporting the **final integrated dataset**

Each notebook handles:

* Loading its raw dataset
* Extracting & resizing images
* Creating its CSV label map
* Saving the processed output

---

## 🎯 Purpose

These scripts exist to:

* Standardize multiple heterogeneous BPA datasets
* Make them suitable for machine learning & forensic analysis
* Ensure reproducibility of the dataset creation pipeline

---
