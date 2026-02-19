# 🎙 Sanskrit Automatic Speech Recognition (ASR)

[![Language](https://img.shields.io/badge/Language-Sanskrit-orange)]
[![Framework](https://img.shields.io/badge/Framework-TensorFlow-blue)]
[![Architecture](https://img.shields.io/badge/Model-CNN--RNN--CTC-purple)]
[![Task](https://img.shields.io/badge/Task-Speech%20Recognition-green)]

An end-to-end Automatic Speech Recognition (ASR) system designed to convert spoken Sanskrit into text, built to address challenges in low-resource language modeling.

---

## 🚀 Project Overview

This project implements a structured ASR pipeline for Sanskrit speech, combining signal processing techniques with deep learning architectures to achieve robust transcription performance across diverse speakers and accents.

### Key Highlights

- 📀 Preprocessed **78 hours** of Sanskrit speech
- 🗣 46,000 sentences from **27 speakers**
- 🧠 CNN–RNN architecture with CTC loss
- 📉 Achieved **7.64% Word Error Rate (WER)** on the evaluation corpus using an end-to-end CNN–RNN–CTC architecture.
- 🔊 Built preprocessing pipelines for accent & dialect variability

---

## 🧠 System Architecture
```
Raw Audio
↓
MFCC Feature Extraction
↓
CNN (Local Feature Learning)
↓
RNN (Temporal Modeling)
↓
CTC Loss
↓
Text Transcription
```
---

### Model Components

- **Feature Extraction:** MFCCs  
- **CNN:** Captures local acoustic patterns  
- **RNN:** Models temporal dependencies in speech  
- **CTC Loss:** Handles unaligned input-output sequences  

---

## 📊 Dataset

- **Total Audio:** 78 hours  
- **Sentences:** 46,000  
- **Speakers:** 27  
  - 20 male  
  - 7 female  
- Native languages: Hindi, Tamil, Kannada, Malayalam, and others  

The dataset was curated to include accent and dialect diversity to improve generalization.

---

## 📈 Results

| Metric | Value |
|--------|--------|
| Baseline WER | 44% |
| Best WER (with augmentation) | 2% |

Data augmentation techniques significantly improved model robustness across speaker variability.

---

## 🛠 Technology Stack

- Python  
- TensorFlow / Keras  
- MFCC Feature Extraction  
- CNN + RNN Architecture  
- Connectionist Temporal Classification (CTC) Loss  
- Evaluation via Word Error Rate (WER)  

---

## 🔧 Engineering Contributions

- Designed structured preprocessing pipeline  
- Built MP3 → WAV conversion workflow  
- Implemented stereo → mono normalization  
- Tuned CNN–RNN architecture for low-resource conditions  
- Applied augmentation techniques to reduce WER  
- Evaluated across multiple dialect groups  

---

## ⚠️ Challenges Addressed

### Low-Resource Language
Limited publicly available Sanskrit speech data required careful dataset construction and preprocessing.

### Accent & Dialect Variability
Model tuning and preprocessing adjustments were required to generalize across speakers with different native language backgrounds.

---

## 🔮 Future Improvements

- Integrate language models for contextual correction  
- Apply SpecAugment & speed perturbation  
- Build real-time inference API  
- Deploy as a scalable transcription service  

---

## 👥 Contributors

- Jayesh Bafana  
- Bijal Bharadva  
- Jay Chaudhari  
- Pranav Dave  
- Vinit Jha  
- Jaanvi Nambiar  

---

### Built to advance speech recognition for low-resource languages.


