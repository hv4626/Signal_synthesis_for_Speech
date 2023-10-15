# Signal_synthesis_for_Speech

This Python script provides a set of functions for speech signal synthesis, which includes generating excitation signals, formant filtering, glottal pulse shaping, and adding noise. These functions can be used to generate and manipulate speech waveforms for various applications, such as speech synthesis and analysis.

## Prerequisites

Before using this code, you should have the following libraries installed:

- Librosa
- Matplotlib
- NumPy
- SciPy
- IPython

You can install these libraries using the following commands:

```bash
pip install librosa
pip install matplotlib
pip install numpy
pip install scipy
pip install ipython
```

## Functions

### 1. `generate_excitation(fs, dur, f0, b, a)`

   - Generates an excitation signal using given parameters.
   - Parameters:
     - `fs`: Sampling frequency
     - `dur`: Duration of the signal
     - `f0`: Fundamental frequency
     - `b` and `a`: Filter coefficients for signal processing

### 2. `sound(f0, f1, b1)`

   - Generates a sound waveform with a linearly varying frequency.

### 3. `glottal_pulse(f0, t)`

   - Generates a glottal pulse waveform.

### 4. `formant_filter(source, freq, t)`

   - Applies a formant filter to the input signal.

### 5. `synthesize_signal(F0, F1, F2, F3, t)`

   - Synthesizes a signal with multiple frequency components.

### 6. `extract_segment(signal, sample_rate, segment_duration)`

   - Extracts a segment from a signal.

### 7. `compute_magnitude_spectrum(signal, window_length, sample_rate)`

   - Computes the magnitude spectrum of a signal.

### 8. `glottal_pulse_shaping(f0, t)`

   - Shapes the glottal pulse using an exponential decay.

### 9. `lip_radiation_filter(source, t)`

   - Applies a lip radiation filter to the input signal.

### 10. `lip_formant_filter(source, freq, t)`

    - Applies a lip formant filter to the input signal.

### 11. `aspiration_noise(signal, intensity)`

    - Adds aspiration noise to the input signal.

### 12. `pitch_jitter(f0, jitter_factor)`

    - Adds pitch jitter to the fundamental frequency.

## Usage

You can use these functions to generate and manipulate speech signals. Make sure to pass the appropriate parameters to each function based on your requirements. Example code for using these functions can be found in the provided Python script.

## Acknowledgments

This code uses various signal processing techniques and is based on libraries like Librosa, NumPy, and SciPy.

## License

This code is provided under the [MIT License](LICENSE.md).

Feel free to modify and use it for your own projects!
