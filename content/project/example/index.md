---
title: Weakly-supervised Anomaly Detection in Surveillance Videos (MSc Thesis)
summary: This project introduces a cutting-edge approach to anomaly detection in urban surveillance systems using Two-Stream Inflated 3D (I3D) Convolutional Networks. By capturing both spatial and temporal features more effectively than traditional methods, our model significantly improves detection precision. Leveraging a weakly supervised Multiple Instance Learning (MIL) framework, we treat surveillance videos as collections of ranked clips, enabling efficient anomaly identification with minimal manual labeling. Optimized for real-world deployment, this scalable and high-performing solution sets new standards in public safety technology through intelligent, context-aware video analysis. [Code](https://github.com/sarehsoltani/Weakly-Supervised-Anomaly-Detection-in-Surveillance-Videos-Based-on-Two-Stream-I3D-ConvNet)
# tags:
#   - Deep Learning
date: '2023-09-1'

# Optional external URL for project (replaces project detail page).
external_link: 'https://arxiv.org/abs/2411.08755'

image:
  # caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

A widespread adoption of city surveillance systems has led to an increase in the use of
surveillance videos in order to maintain public safety and security. This thesis tackles the
problem of detecting anomalous events in surveillance videos. The goal is to automatically
identify abnormal events by learning from both normal and abnormal videos. Most previous
works considered any deviation from learned normal patterns as an anomaly. However, this
may not always be valid since the same activity could be normal or abnormal under different
circumstances. To address this issue, this thesis utilized Two-Stream Inflated 3D (I3D) Convolutional Networks to extract spatial and temporal video features and demonstrated how it
outperformed the 3D Convolutional Network (C3D) used in prior work as a feature extractor.
To avoid annotating abnormal activities in training videos, a weakly supervised anomaly detection model was implemented based on the Multiple Instance Learning (MIL) framework. The
model considers normal and abnormal videos as bags and video clips as instances. It learns a
ranking model to predict high anomaly scores for video clips containing anomalies. The thesis
further shows that the choice of features input, such as concatenating RGB and Flow features,
and careful choice of optimization settings, such as optimizer, can significantly improve the
performance of the anomaly detection model on some evaluation metrics.