# SUB-CONVOLUTIONAL-VASNet-BASED-SPEECH-ENHANCEMENT

#  Audio Noise Reduction using Python

This project demonstrates audio noise reduction using Python libraries such as `librosa`, `noisereduce`, and `soundfile`. The code loads an MP3 audio file, adds synthetic and real-world noise (like cafe background sounds), and applies both stationary and adaptive noise reduction techniques.

##  Project Structure

- Load and visualize original audio waveform
- Add real-world noise from an online source
- Apply stationary and adaptive noise reduction
- Visualize and playback both noisy and cleaned audio

##  Requirements

These libraries are required to run this project:

```bash
pip install librosa noisereduce soundfile matplotlib
```

>  If you're running this in **Google Colab**, the script checks for the environment and installs missing packages automatically.

##  Input

Replace this file path with your own MP3 file:

```python
mp3_file = "/content/WhatsApp Audio 2024-10-24 at 13.43.58_e98e5504.mp3"
```

##  Usage Steps

1. **Load the Audio**
   - Uses `librosa.load()` to import the audio file while preserving its original sample rate.

2. **Plot and Play Original Audio**
   - Plots waveform using `matplotlib`
   - Plays audio inline using IPython

3. **Add Cafe Noise**
   - Downloads a real-world background noise sample (cafe ambiance)
   - Matches the duration with the original audio
   - Adds noise with a specific signal-to-noise ratio (SNR)

4. **Stationary Noise Reduction**
   - Applies `noisereduce.reduce_noise` with `stationary=True` to reduce static noise

5. **Adaptive Noise Reduction**
   - Uses `prop_decrease=0.9` for stronger adaptive noise suppression
   - Visualizes and plays the enhanced audio

## Key Features

- Visualizes audio waveforms before and after denoising
-  In-browser playback using IPython widgets
-  Supports real-world noise simulation
- Applies both stationary and adaptive denoising techniques

##  Example Outputs

- Waveform plots of:
  - Original Audio
  - Noisy Audio (with cafe noise)
  - Stationary Noise-Reduced Audio
  - Adaptive Noise-Reduced Audio
- Inline audio players for all versions

## Notes

- This code works best in **Google Colab** or any Python environment with Jupyter Notebook support.
- If using other MP3 files, ensure the file exists at the specified path or upload it in Colab using the file upload widget.


##  Author

Adipareddy Surya Prakash Reddy  
BTech CSE (Data Science), Kalasalingam Academy of Research and Education

feel free to reach out suryaprakash81293@gmail.com

