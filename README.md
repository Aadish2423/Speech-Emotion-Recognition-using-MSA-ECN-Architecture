# Speech Emotion Recognition using MSA-ECN Architecture

## Overview

Speech Emotion Recognition (SER) is an important task in human–computer interaction that aims to identify human emotions from speech signals. This project presents an advanced deep learning–based SER system using a **Multi-Scale Attention-based Capsule Network (MSA-ECN)** architecture.

The model combines **multi-channel acoustic feature extraction, convolutional learning, attention mechanisms, and capsule networks** to effectively capture both low-level and high-level emotional patterns in speech.

The architecture is designed to model **spectral features, temporal dependencies, and feature relationships**, achieving an accuracy of approximately **85%**.

---

## Objectives

- Develop a robust system to classify emotions from speech signals  
- Capture diverse acoustic properties using multi-channel feature extraction  
- Model both local and long-range temporal dependencies in audio  
- Leverage capsule networks to improve feature–emotion relationships  
- Achieve high accuracy and generalization in emotion classification  

---

## Model Architecture (MSA-ECN)

### 🔹 Multi-Channel Feature Extraction
- Extract acoustic features such as **MFCC, Mel Spectrogram, and Chroma**  
- Combine them as multi-channel inputs  
- Capture complementary information like pitch, tone, and frequency variations  

---

### Multi-Scale CNN Encoder
- Uses convolutional layers with different kernel sizes  
- Captures:
  - Fine-grained details (small kernels)  
  - Global patterns (large kernels)  
- Produces rich **spectro-temporal representations**  

---

### Conformer-Based Attention Encoder
- Combines **self-attention** and **convolution modules**  
- Learns:
  - Long-range dependencies (attention)  
  - Local patterns (convolution)  
- Helps model how emotions evolve over time  

---

###  Hierarchical Capsule Network
- Primary capsules capture low-level speech features  
- Emotion capsules represent different emotion classes  
- Uses **dynamic routing** to learn relationships between features and emotions  

---

### Emotion Classification
- Each capsule outputs a vector  
- The **vector length represents probability** of an emotion  
- Emotion with the highest activation is selected as final prediction  

---

## Methodology

### 1. Audio Preprocessing
- Load and normalize speech signals  
- Remove noise and inconsistencies  
- Extract relevant speech segments  

### 2. Feature Extraction
- Extract MFCC, Mel Spectrogram, and Chroma features  
- Stack features into multi-channel inputs  
- Convert into model-ready format  

### 3. Model Training
- Train the MSA-ECN architecture end-to-end  
- Optimize using backpropagation  
- Learn hierarchical and temporal representations  

### 4. Evaluation
- Evaluate model performance on test data  
- Achieved approximately **85% accuracy**  
- Analyze performance across emotion classes  

---

## Tech Stack

- Python  
- PyTorch / TensorFlow  
- Librosa  
- NumPy  
- Scikit-learn  
- Google Colab  

---

## Results & Observations

- Multi-channel features improve speech representation  
- Multi-Scale CNN captures both local and global patterns  
- Conformer enhances temporal understanding of emotions  
- Capsule Networks improve feature–emotion relationships  
- Achieved **~85% accuracy**, showing strong performance  

---

## Future Enhancements

- Apply **data augmentation techniques**  
- Explore **CNN + Transformer hybrid models**  
- Fine-tune Conformer and Capsule Network parameters  
- Implement real-time emotion recognition  
- Deploy as a **web or desktop application**  

---

## Author

**Aadish Bane**  
*Interests: Artificial Intelligence, Machine Learning, Deep Learning*
