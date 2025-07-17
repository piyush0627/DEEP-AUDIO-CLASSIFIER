# Deep Audio Classifier

A comprehensive deep learning project for classifying environmental audio sounds using Convolutional Neural Networks (CNN) and mel-spectrograms. This project uses the UrbanSound8K dataset to classify 10 different types of urban environmental sounds.

##  Project Overview

This project implements a CNN-based audio classifier that:
- Processes raw audio files into mel-spectrograms
- Uses a deep CNN architecture for feature learning
- Classifies environmental sounds into 10 categories
- Achieves robust performance with proper regularization
- Provides real-time prediction capabilities

##  Dataset

**UrbanSound8K Dataset**
- **Size**: ~8,732 audio files
- **Classes**: 10 urban environmental sound categories
  - Air conditioner
  - Car horn
  - Children playing
  - Dog bark
  - Drilling
  - Engine idling
  - Gun shot
  - Jackhammer
  - Siren
  - Street music
- **Format**: Various audio formats (WAV, MP3, etc.)
- **Duration**: Variable length audio clips
- **Source**: Automatically downloaded from Zenodo

### Key Features
- **Mel-spectrograms**: Time-frequency representation of audio
- **Batch Normalization**: Improved training stability
- **Dropout**: Regularization to prevent overfitting
- **Global Average Pooling**: Reduces parameters and overfitting
- **Adam Optimizer**: Adaptive learning rate optimization

##  Performance

### Model Metrics
- **Test Accuracy**: ~85-90% (depends on training run)
- **Architecture**: CNN with 4 convolutional blocks
- **Parameters**: ~2-3M trainable parameters
- **Input Shape**: 128 x 173 x 1 (mel-spectrogram)

### Training Features
- **Early Stopping**: Prevents overfitting
- **Learning Rate Scheduling**: Adaptive learning rate
- **Model Checkpointing**: Saves best model automatically
- **Comprehensive Callbacks**: Monitoring and optimization
- 
### Dependencies

librosa==0.9.2      
tensorflow>=2.8.0  
scikit-learn>=1.0   
matplotlib>=3.5.0 
seaborn>=0.11.0     
numpy>=1.21.0       
pandas>=1.3.0       
