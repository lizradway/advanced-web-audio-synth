# 🎹 Web Audio Synthesizer

An interactive **browser-based synthesizer** built with the **Web Audio API**.
This project allows users to play musical notes using their **computer keyboard** while experimenting with multiple **sound synthesis techniques** and audio modulation effects.

The synthesizer supports **additive synthesis, amplitude modulation (AM), and frequency modulation (FM)**, along with configurable parameters such as waveform type, oscillator count, and modulation frequency.

---

# Features

### 🎹 Keyboard Piano

Play musical notes using your **computer keyboard**, mapped to standard musical frequencies.

### 🔊 Multiple Synthesis Methods

The synthesizer supports three synthesis techniques:

* **Additive Synthesis** – Combines multiple oscillators to build richer sounds
* **Amplitude Modulation (AM)** – Modulates the amplitude of a carrier signal
* **Frequency Modulation (FM)** – Modulates the frequency of a carrier signal to produce complex tones

### 🎛 Sound Controls

Users can adjust several sound parameters:

* **Waveform type**

  * Sine
  * Square
  * Sawtooth
  * Triangle

* **Number of oscillators** (Additive synthesis)

* **Modulation frequency** (AM / FM synthesis)

* **Low Frequency Oscillator (LFO)** for vibrato effects

### 🎵 Polyphonic Playback

Multiple notes can be played simultaneously.


---

# Keyboard Layout

The keyboard is mapped similarly to a piano layout.

Lower row:

```
Z  S  X  D  C  V  G  B  H  N  J  M
C  C# D  D# E  F  F# G  G# A  A# B
```

Upper row:

```
Q  2  W  3  E  R  5  T  6  Y  7  U
```

Each key corresponds to a specific musical frequency.

---

# How It Works

The synthesizer uses the **Web Audio API** to generate and manipulate sound.

Key components include:

### AudioContext

The main audio engine responsible for processing and routing sound.

### OscillatorNode

Generates the sound waves used to produce musical notes.

### GainNode

Controls the volume of individual signals and the overall output.

### Modulation

* **AM synthesis** modulates amplitude using another oscillator.
* **FM synthesis** modulates frequency using another oscillator.
* **LFO** adds low-frequency modulation for vibrato effects.

To prevent distortion, the program automatically adjusts **global gain levels** when multiple oscillators are active.


# License

This project is intended for **educational and experimental use**.
Feel free to modify and extend it.
