# LSTM-Based Music Generation

This project demonstrates how to generate music using a Long Short-Term Memory (LSTM) neural network trained on classical MIDI files. It uses PyTorch and processes MIDI data using `pretty_midi`. The model predicts musical pitch, step (inter-note timing), and duration for generating new melodies.

## Dataset

- The training data consists of MIDI files from classical composers (e.g., Mozart).
- Files are extracted and processed using `pretty_midi`.

## Features

- Converts MIDI to note sequences with pitch, step, and duration.
- Prepares time-series data for LSTM input.
- Trains a multi-layer LSTM network to predict the next note.
- Generates new musical sequences.
- Converts predicted sequences back into playable MIDI format.
- Includes utilities to play generated audio in a notebook.

## Model Architecture

- 3-layer LSTM network
- Dropout regularization
- Dense outputs for pitch (classification), step and duration (regression)
- Loss: weighted combination of CrossEntropy and MSE

## Dependencies

Install the following before running the notebook:

pip install pretty_midi
sudo apt install -y fluidsynth
pip install --upgrade pyfluidsynth

## Acknowledgments
Based on techniques from Google's Magenta project

Inspired by classical music generation papers and open-source MIDI datasets

## Contact
Feel free to raise issues or drop a mail at asitrath1111@gmail.com.
