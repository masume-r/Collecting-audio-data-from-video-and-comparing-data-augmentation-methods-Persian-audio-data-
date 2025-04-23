# Collecting-audio-data-from-video-and-comparing-data-augmentation-methods-(Persian-audio-data)

## 📌 Overview

This project explores how to collect and process voice segments from Persian-language films, and how different audio data augmentation methods impact the performance of emotion classification models.

Our goal is to test and compare augmentation techniques such as:
- Adding background noise
- Pitch shifting
- Time stretching
- Random mixed augmentation

We use Mel Spectrograms as the visual representation of audio, and train CNN-based models for emotion classification.

## 🎯 Objectives

- Extract dialogue audio from Persian movie
- Split speech into segments using silence detection
- Manually label the emotional tone of segments into 4 classes:
  - 0: Neutral
  - 1: Happy
  - 2: Sad
  - 3: Angry
- Apply various audio augmentation methods
- Generate Mel Spectrograms from each version
- Train and evaluate CNN models (e.g., ResNet18)
- Visualize results using accuracy plots and confusion matrices


## 🗂️ Project Structure

fa-audio-augmentation/ ├── README.md ├── requirements.txt ├── notebooks/ │ ├── 01_data_collection.ipynb │ ├── 02_silence_segmentation.ipynb │ ├── 03_augmentation_noise.ipynb │ ├── 04_augmentation_pitch.ipynb │ ├── 05_augmentation_stretch.ipynb │ ├── 06_augmentation_mixed.ipynb │ ├── 07_melspectrogram_generation.ipynb │ └── 08_model_training.ipynb ├── results/ │ ├── accuracy_plots/ │ ├── confusion_matrices/ │ └── summary_metrics.csv ├── models/ │ └── best_model_noise.pth ├── utils/ │ ├── audio_utils.py │ └── plot_utils.py └── .gitignore
