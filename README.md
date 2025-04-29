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


## 🛠️ Installation

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/masume-r/Collecting-audio-data-from-video-and-comparing-data-augmentation-methods-Persian-audio-data-.git

cd comparing-data-augmentation-methods
pip install -r requirements.txt







## 🗂️ Project Structure
comparing-data-augmentation-methods/ ├── notebooks/ # All Jupyter notebooks for each step │ ├──
 01_data_collection.ipynb │ ├── 02_silence_segmentation.ipynb │ ├── 03_create_csv_from_segments.ipynb │ ├── 04_clean_and_balance_labeled_data.ipynb │ ├── 05_split_final_data.ipynb │ ├── 06_data_augmentation_final_fixed.ipynb │ ├── 07_generate_melspectrogram.ipynb │ ├── 08_prepare_augmented_csvs.ipynb │ ├── 09_prepare_test_data.ipynb │ ├── 10_Train_a_Model_(ResNet18_Fine_Tuning).ipynb │ ├── 11_Train_a_Model_(ResNet18_Fine_Tuning)Noise_aug.ipynb │ ├──  12_Train_a_Model(ResNet18_Fine_Tuning)pitch_aug.ipynb │ ├── 13_Train_a_Model(ResNet18_Fine_Tuning)stretched_aug.ipynb │ ├── 14_Train_a_Model(ResNet18_Fine_Tuning)_Mixed_Augmentation.ipynb │ └── visualization.ipynb ├── requirements.txt # List of required Python packages ├── README.md # Project documentation (this file)


 
---

## 🛠️ Main Dependencies

- Python 3.8+
- PyTorch
- torchvision
- torchaudio
- librosa
- matplotlib
- seaborn
- scikit-learn
- pandas
- numpy

All dependencies can be installed using:

```bash
pip install -r requirements.txt



## 📊 Results Overview

- Evaluated the effect of four different audio augmentation methods on emotion classification.
- Trained models using fine-tuned ResNet18 architecture.
- Visualized performance through confusion matrices and accuracy plots.
- Mixed augmentation showed slightly better generalization than individual methods.

evaluated each augmentation method by training a ResNet-18 model on the augmented datasets and measuring its best test accuracy. The comparison results are presented below.

### 📋 Accuracy Table

![Accuracy Table](notebooks/table.png)

### 📈 Accuracy Comparison (Bar Chart)

This bar chart shows the best test accuracy achieved by each augmentation strategy:

![Accuracy Bar Chart](notebooks/plt.png)

### 📉 Training Loss Over Epochs

This line chart visualizes how the training loss decreased over epochs for each version of the dataset:

![Training Loss](notebooks/plt-loss.png)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to open issues, create pull requests, or suggest improvements to make this project better.

---

## ✨ Acknowledgements

- Thanks to SeoulTech DS Lab for support and resources.
- Special thanks to the open-source community and libraries such as PyTorch, torchvision, torchaudio, librosa, and scikit-learn.







