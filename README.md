# naversia-voice-recorder

This is a simple voice recorder that captures audio from the microphone and saves it as a WAV file. The program uses the PyAudio library to access the microphone and record the audio. It also uses threading to run the recording process in the background so that the user interface remains responsive. The Tkinter library is used to create the graphical user interface.

Requirements:
To run this program, you need to install the following libraries:

    PyAudio
    Tkinter

Usage:

    Run the program.
    Click on the microphone icon to start recording.
    Click on the microphone icon again to stop recording.
    The recording will be saved in the same directory as the program with the name "recordingX.wav", where X is a unique number.

Code Explanation:

    Import the required libraries: os, wave, time, threading, tkinter, and pyaudio.
    Create a class named "VRecorder".
    In the init() method, create a window using Tkinter and add a button and a label to it.
    Create a click_handler() method that toggles the recording state and changes the color of the button accordingly.
    Create a record() method that uses PyAudio to record the audio from the microphone and save it as a WAV file.
    Use threading to run the record() method in the background.
    Create an instance of the VRecorder class to start the program.

Limitations:

    The program only records mono audio with a sample rate of 44100 Hz and a sample size of 16 bits.
    The program may not work with all microphones, depending on their compatibility with PyAudio.
    The program does not include any error handling or user feedback in case of errors.

Improvements:

    Add support for stereo audio and other sample rates and sample sizes.
    Add error handling and user feedback for errors.
    Add a feature to play back the recorded audio.
    Add a feature to delete recordings.
