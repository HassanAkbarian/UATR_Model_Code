# UATR_Model_Code
Underwater Acoustic Target Recognition (UATR) – Signal Processing and ROI Extraction

This repository provides a collection of Python scripts used for preprocessing, analyzing, and visualizing underwater acoustic signals. The methods implemented here are designed to support research in Underwater Acoustic Target Recognition (UATR) by enhancing feature extraction from ship-radiated sound signals using spectrogram-based representations.

📘 Overview

The primary focus of this project is to improve the classification accuracy of underwater acoustic targets (e.g., ships) by extracting and highlighting meaningful signal segments while discarding irrelevant or noisy parts. Through spectrogram analysis, silence removal, and double-threshold energy filtering, this codebase helps in identifying acoustic Regions of Interest (ROIs) suitable for deep learning models such as 1D and 2D MobileNet.

🎯 Key Features

Resampling of audio signals to a consistent sampling rate (e.g., 22050 Hz).

Silence Removal based on short-term energy detection.

Spectrogram Calculation using Short-Time Fourier Transform (STFT).

ROI Extraction via energy-based double-threshold masking.

Bounding Box Visualization on spectrograms using OpenCV and Matplotlib.

Grayscale ROI Image Export for downstream machine learning applications.

🔬 Research Context

This repository is part of an ongoing research project focused on lightweight and efficient machine learning models for underwater acoustic classification. The approach relies on accurate spectrogram-based representations, where only the most informative portions of the acoustic signal are used to train and evaluate deep learning classifiers under real-world noisy marine conditions.

📂 Project Structure

├── resample_wavs.py         # Resample audio files to target sample rate
├── silence_removal.py       # Remove silent parts from .wav files
├── roi_extraction.py        # Identify and extract Regions of Interest in spectrogram
├── roi_visualization.py     # Visualize and export bounding boxes over spectrograms
├── audio_samples/           # Example audio files (not included)
└── output_images/           # Output spectrogram images with ROI boxes

🛠 Requirements

librosa

numpy

matplotlib

opencv-python

scipy

tqdm

pyAudioAnalysis

Install them via pip:

pip install librosa matplotlib opencv-python numpy scipy tqdm pyAudioAnalysis

📄 Citation

If you use this code for your research or publication, please cite our related paper:

Akbarian, H. et al. (2025). Underwater Acoustic Target Recognition Using Spectrogram ROI Approximation and Modified MobileNet Networks. [DOI or conference info here]

📬 Contact

For questions, suggestions, or collaborations, please contact:

Hassan Akbarian[Akbarian.hassan@gmail.com][Sahand University of Technology, Tabriz, Iran ]

Thank you for using and supporting this research!

