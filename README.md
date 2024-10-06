# Text-to-Speech with Torchaudio

This repository contains a Jupyter Notebook that demonstrates how to implement a Text-to-Speech (TTS) system using PyTorch and Torchaudio. The notebook walks through key steps of processing text input, generating speech from it, and training a neural network for TTS purposes.

## Features
- **Torchaudio Integration**: Leverages PyTorch's audio processing library to handle data and audio manipulation.
- **Neural Network-Based TTS**: Builds a neural network architecture for converting text input to speech using Tacotron 2-like architecture.
- **Spectrogram Generation**: Uses spectrograms as an intermediate representation of speech for TTS.
- **WaveNet Vocoder**: A WaveNet-based vocoder generates the final waveform from mel spectrograms.
  
## Requirements
To run the notebook, you will need the following dependencies:

- Python 3.7+
- PyTorch 1.7+
- Torchaudio
- Jupyter Notebook
- NumPy
- Matplotlib

## Notebook Overview
- Text Processing: The notebook starts by preprocessing the input text into a suitable format for the TTS system.
- Tacotron 2 Architecture: It covers the implementation of the Tacotron 2 architecture, which generates mel spectrograms from text sequences.
- Vocoder Integration: A WaveNet vocoder is used to generate audio waveforms from the mel spectrograms.
- Training and Inference: It includes sections for training the model and performing inference for new text inputs.
- You can install the required packages using:
- ```bash
pip install torch torchaudio jupyter numpy matplotlib

## Data
To train the model, you can use public datasets like:

LJ Speech Dataset , 
Mozilla Common Voice ([URL](https://commonvoice.mozilla.org/en))
( Please follow the dataset's licensing requirements. )

## Acknowledgements
The architecture is inspired by [Tacotron 2](https://arxiv.org/abs/1712.05884) and [WaveNet papers](https://arxiv.org/abs/1609.03499)
PyTorch and Torchaudio provide the core libraries used in this project.
