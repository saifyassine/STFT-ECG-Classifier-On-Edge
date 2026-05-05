# ECG Arrhythmia Classification using STFT-CNN with Pruning & Quantization

Deep learning pipeline for ECG arrhythmia detection optimized for edge devices (Raspberry Pi, mobile). Achieves 98.66% accuracy with models as small as 5KB and < 1ms inference time.

## 📋 Overview

This project implements a complete pipeline for ECG arrhythmia classification on the MIT-BIH dataset:

1. **Signal Processing**: Resampling, R-peak detection, beat segmentation, RR-interval extraction
2. **Model Architecture**: STFT-based CNN with trainable FIR filter bank (4 variants)
3. **Optimization**: Magnitude-based pruning (30-60% sparsity) + Quantization (float16/int16/int8)
4. **Edge Deployment**: Implementation code on RaspberryPi 3 Model B.

