Audio Deepfake Detection using Paralinguistic Learning

This repository contains the research paper and implementation for “Audio Deepfake Detection using Paralinguistic Learning”, authored by Melvin V, Department of Computer Science, St. Joseph’s University, Bengaluru, India.

Abstract

Modern AI speech synthesis frameworks such as WaveNet, Tacotron 2, and GAN-based voice models can now generate highly realistic synthetic voices, posing risks of misinformation, impersonation, and identity theft.
This research proposes a multi-feature deepfake detection framework that combines acoustic, temporal, prosodic, glottal, and paralinguistic features to robustly identify manipulated or AI-generated speech.

Key extracted features include:

Acoustic: MFCCs, spectral centroid, spectral flux

Temporal: Zero-Crossing Rate (ZCR), Short-Time Energy (STE)

Prosodic: Pitch, intensity, and speech rate

Glottal: Harmonic-to-Noise Ratio (HNR), Normalized Amplitude Quotient (NAQ)

Paralinguistic: TRILLsson embeddings capturing rhythm, stress, and emotional tone

These features are fused and processed using LSTM autoencoders and DNN-based fusion networks with attention layers. The system achieved:

98.1 % accuracy

15 % reduction in Equal Error Rate (EER)
compared to MFCC-only baselines, showing superior robustness to unseen spoofing attacks.

Core Technologies

Python, TensorFlow / PyTorch

Librosa, TRILLsson, NumPy, Pandas

ASVspoof and WaveFake datasets

LSTM Autoencoder, DNN Attention Fusion

Highlights

Multi-feature fusion improves generalization to unseen deepfake types

Paralinguistic embeddings enhance discrimination of emotional and rhythm patterns

Strong results on benchmark datasets with state-of-the-art accuracy

Extensible for real-time, mobile, and multi-modal (audio + video) detection

Repository Structure Example
Audio-Deepfake-Detection/
│
├── paper/
│   └── Audio_Deepfake_Detection_using_Paralinguistic_Learning.pdf
│
├── code/
│   ├── feature_extraction.py
│   ├── model_training.py
│   ├── evaluation.py
│   └── requirements.txt
│
├── data/ (optional sample clips)
│
├── README.md
└── LICENSE

🧑‍💻 Author

Melvin V
M.Sc. Computer Science — St. Joseph’s University
📧 melvinvenk707@gmail.com
