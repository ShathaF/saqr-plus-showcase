# SAQR+ | Smart Crowd Monitoring System

A graduation project that counts people in crowded scenes in real time, to support crowd monitoring in stadiums and large venues. **2nd place at the "Nahnu Hona 4" Graduation Projects Exhibition, Taibah University, 2026.**

> **This repository is a project showcase.** The source code and trained model weights are not published because the project is owned by the university.

## Videos

| Project introduction | Live demo |
|:---:|:---:|
| [![SAQR+ introduction](docs/intro-thumbnail.png)](https://youtu.be/9INMoCznNrg) | [![SAQR+ demo](docs/demo-thumbnail.png)](https://youtu.be/CM7lS4D2KUA) |

## The problem

Knowing how many people are in a space, as it happens, is essential for safety and crowd management in places like stadiums. Counting manually does not scale, so SAQR+ automates it from video.

## The solution

**SaqrNet** is a modified convolutional neural network built in PyTorch for crowd counting. It is deployed for real-time video monitoring on stadium footage.

## Results

Evaluated on the public **ShanghaiTech Part B** benchmark against the **CSRNet** baseline (lower is better):

| Model | MAE | MSE |
|-------|----:|----:|
| CSRNet (baseline) | 10.6 | 16.0 |
| **SaqrNet (ours)** | **10.32** | **15.80** |

- **2.6% lower MAE** than the baseline.
- **9.25 FPS** real-time inference on stadium footage.

## Data pipeline

Beyond the public benchmark, the team built a preprocessing and annotation pipeline with OpenCV and Pandas, using footage collected locally from a sports club in Yanbu.

## My role

I led a 5-member team: I coordinated tasks, handled communication with academic supervisors, and delivered the project on schedule. I also designed and trained the model and built the data pipeline.

## Tech stack

Python · PyTorch · OpenCV · Pandas · NumPy · Computer Vision · CNN · Google Colab · Kaggle

## Follow the project

- X (Twitter): [@Saqr_plus](https://x.com/Saqr_plus)

## Author

**Shatha Alluhaibi**, Information Systems graduate, Taibah University (College of Computer Science and Engineering).
See my other project: [Secure Password Validator](https://github.com/ShathaF/secure-password-validator).

---

*All rights reserved. The videos, images and text in this repository are shared for portfolio purposes.*
