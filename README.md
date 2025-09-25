# YouTube Video View Prediction and Optimization Guide

## 📌 Project Overview

This project aims to help YouTube creators optimize their video settings (such as thumbnails, titles, and publish time) in order to maximize views. We build a predictive model that provides actionable, data-driven insights for both new and established creators.

## 🎯 Business Goal

Provide actionable insights to guide YouTube creators in optimizing their video settings to increase views.

## 💡 Motivation & Novelty

* YouTube is highly competitive, and small optimizations can lead to significant increases in engagement.
* Our project integrates structured and unstructured data (thumbnails, titles, metadata) into a **multi-modal deep learning model**.
* This approach is relatively new in offering comprehensive, data-driven recommendations for video optimization.

## 📊 Data Collection

**Source:** YouTube.com (via YouTube API)

* **Unstructured Data:**

  * Video titles (text)
  * Video thumbnails (images)
* **Structured Data:**

  * Publish time of each video
  * Views per video
  * Likes per video
  * (Planned) Number of subscribers per channel
  * (Planned) Video category

➡️ Note: The YouTube API allows up to 10,000 rows of data per account per day.

## 🎯 Prediction Goal

Build a **multi-modal deep learning model** that predicts the view count of YouTube videos and identifies which features (thumbnail design, title, metadata) have the strongest impact on views.

* **Predictors:** Thumbnails, titles, publish time, video category, number of subscribers.
* **Label:** View count of the YouTube video.

## ⚙️ Methodology

We use a **multi-model deep learning architecture** with the Functional API:

1. **Thumbnail Feature Extraction**

   * CNNs process video thumbnails to extract visual features.

2. **Textual Feature Extraction**

   * NLP techniques process video titles and generate embeddings.

3. **Structured Data Processing**

   * Metadata (publish time, likes, subscribers, etc.) passes through dense layers.

4. **Fusion & Prediction**

   * Features from all sources are combined and passed through fully connected layers to predict view counts (continuous values).

## 👥 Team Members

* Shuomeng Guan
* Manyi Hong
* Wenxin Liang
* Zehui Wang

---

📌 *This project is part of BA865 Team 07 coursework. The final deliverable will include data pipelines, model training, evaluation, and an optimization guide for YouTube creators.*

