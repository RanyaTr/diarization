# Whisper Diarization Project

## Description:

This project uses OpenAI's Whisper API and Hugging Face's transformer and dataset libraries to perform automatic transcription and diarization of audio. Diarization helps segment audio to identify different speakers and improve audio content analysis.


## Prerequisites:

Before running this project, make sure the following dependencies are installed:

- Python 3.11.9
- ffmpeg
- git
- The necessary Python libraries (see below).

## Installation instructions

1- Installing Whisper:


`pip install git+https://github.com/openai/whisper.git`

2- Installation of dependencies:

`pip install openai`

3- Installation de numpy, librosa,torchmetrics,transformers
```
 pip install numpy
 pip install librosa
 pip install torchmetrics
 pip install transformers
 pip install Levenshtein
```


## Use
Import the necessary modules, including WhisperProcessor and WhisperForConditionalGeneration from transformers.
Configure transcription settings and run audio processing to generate text with speaker segmentation.

## Features
- **Automatic Speech Transcription:** Transcribes audio files into text format.
- **Speaker Diarization:** Identifies and segments different speakers in the audio, making it easier to distinguish between them.
- **Structured Output:** Exports transcription results in a structured format for further analysis or integration with other tools.
- **Audio Preprocessing:** Converts audio to a 16kHz sample rate for compatibility with transcription and diarization models.

## Remarks
This project requires `ffmpeg` for audio manipulation, as well as converting the rate of audios to 16kHz by the command :
`ffmpeg -i input_audio.wav -ar 16000 output_audio_16khz.wav`
