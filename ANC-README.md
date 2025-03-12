 Adaptive Noise Cancellation (ANC) Using LMS Algorithm

Designed and implemented an adaptive noise cancellation system in MATLAB to remove noise from audio signals using the Least Mean Squares (LMS) algorithm.
Generated reference noise signals, applied adaptive filtering, and analyzed the performance of the system.
Visualized and compared noisy and denoised audio signals using time-domain plots.
Gained hands-on experience with MATLAB’s audio processing tools (audioread, sound, dsp.LMSFilter) and adaptive filtering techniques.

The key steps in the MATLAB code are:

Loading the Audio File: It loads an audio file named you belong with me noisy.mp4.
Stereo to Mono Conversion: If the audio is in stereo, it converts it to mono.
Noise Segment Extraction: It extracts a noise segment from the audio.
Adaptive Noise Cancellation: It applies an LMS (Least Mean Squares) filter to perform adaptive noise cancellation on the audio.
Result Visualization: It plots the original and filtered audio signals for comparison.
