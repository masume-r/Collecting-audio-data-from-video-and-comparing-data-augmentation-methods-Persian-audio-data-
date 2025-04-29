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

- 
## 🛠️ Installation

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/masume-r/Collecting-audio-data-from-video-and-comparing-data-augmentation-methods-Persian-audio-data-.git



