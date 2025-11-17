# Blood Pattern Image Dataset

This dataset contains **283 blood pattern images** collected, processed, and integrated from multiple sources to support research in **bloodstain pattern analysis (BPA)** and **computer vision applications**.

## 📁 Dataset Structure

* **Folder:** `Blood Images/`
  Contains all processed blood pattern images.
* **CSV File:** `path.csv`
  Includes two columns:

  * **Image** – the image filename
  * **Class** – the blood pattern category for each image

## 🖼️ Image Details

All images were standardized and preprocessed to ensure consistency and easy model training:

* **Resolution:** `224 × 224`
* **Background:** Pure **white background**
* **Content:** Only the blood pattern is present on the white background
* **Resource Friendly:** Resizing helps train deep learning models on low-resource environments

## 🩸 Included Blood Pattern Types

The dataset includes a curated selection of forensic-relevant blood patterns:

* **Gunshot patterns** (high-velocity impact)
* **Beating/Blunt force patterns**
* **Blood drips on paper** (gravity-driven patterns)

## 🎯 Purpose

This dataset is designed for:

* Deep learning model training
* Forensic image analysis research
* Pattern recognition projects
* Educational use in BPA and computer vision domains

