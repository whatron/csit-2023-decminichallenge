# CSIT 2023 - Audio Processing Mini Challenge

This repository contains code and materials related to the Data Science in Audio Processing and Manipulation mini challenge for CSIT 2023.

## How to View

To view the Jupyter Notebook for this mini challenge, please follow this [link](https://github.com/whatron/csit_2023decminichallenge/blob/main/answers.ipynb).

Or,

To play the audio content inline within the Jupyter Notebook, follow these steps:

1. Download the [answers.ipynb](https://github.com/whatron/csit_2023decminichallenge/blob/main/answers.ipynb) Jupyter Notebook provided in the repository.
2. Run Jupyter Notebook on your local machine.
3. Open the downloaded Jupyter Notebook file.
4. Navigate to the relevant sections containing audio visualizations or analyses.

## Tasks

### Task 1
Provided with an audio file T1_audio.wav.\
Simply reverse and speed up the audio using the `librosa` library.

### Task 2
Provided with 4 audio files.\
Display the spectrogram using `librosa.display.specshow`.\
There is text noticable within the spectrograms.

### Task 3
Provided with an audio file C.Noisy_Voice.wav.\
The spectrogram show that the noise is present exclusively at frequencies above 2000 Hz, as well as below 100 Hz.\
Filter the audio using `butter` from `scipy.signal`.\
Apply Short-Time Fourier Transform (STFT) using `stft` from `scipy.signal` to clean up the remainding audio waveform.\
Normalize the audio as it is too quiet.\
Using `openai-whisper`, we can detect the language of the audio, and translate the audio.
```bash
whisper Task_3/output.wav --model large-v2 --task translate
```


