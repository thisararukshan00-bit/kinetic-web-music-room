# 🎸🥁 Kinetic Web Music Room

An interactive, physics-driven multi-instrument web music studio and real-time sheet music transcriber. Built entirely inside a single HTML file with zero external audio dependencies.

🔗 **[Play the Live Demo Here!](https://thisararukshan00-bit.github.io/kinetic-web-music-room/)**

---

## ✨ Key Features

* **3 Simultaneous Instrument Zones:**
  * **1️⃣ Strings (Left Zone):** Switch between *Acoustic Guitar, Electric Guitar, Mandolin (double-coursed)*, and *Violin*. Strum directly with your cursor or touch.
  * **2️⃣ Melody (Center Zone):** Play or bounce notes across a *Yamaha Synth Keyboard, Grand Piano, Bansuri Flute*, or *Brass Trumpet*.
  * **3️⃣ Rhythm & Percussion (Right Zone):** Switch between a realistic *Acoustic Drum Kit, Roland-style 8-pad Octapad*, and traditional Sri Lankan/Indian Percussion (*Geta Bera, Yak Bera, Tabla, Thalampata*).
* **Kinetic Physics Sequencer:** Launch glowing orbs across the stage. Whenever an orb crosses a string or collides with a drum/melody pad, it plucks the note and triggers visual vibrations!
* **Custom Drag & Drop Layout:** Reposition drums and melody nodes anywhere on the screen to design custom bounce paths and automated rhythmic loops.
* **Live Sheet Music Transcription:** Every note played (manually or via kinetic orbs) is transcribed in real-time onto a scrolling musical staff at the bottom.

---

## 🛠️ How It Was Built (Architecture & Tech Stack)

This project was developed through conversational AI-assisted creative coding using **Gemini** and relies 100% on native web technologies without any external libraries or MP3/WAV samples:

1. **Web Audio API (Real-Time Audio DSP):**
   * **Karplus-Strong String Synthesis:** Simulates physical string vibrations using a delay-line ring buffer and low-shelf body resonance filters for realistic guitar and mandolin plucks.
   * **Synthesized Percussion & Winds:** Uses custom oscillator envelopes, filtered noise bursts, and vibrato LFOs to synthesize drums, octapad hits, Sri Lankan traditional drums, flutes, and brass instruments on the fly.
2. **HTML5 Canvas (60 FPS Rendering & Physics):**
   * Handles real-time line-segment intersection math (detecting when an orb crosses a string), circular/rectangular elastic collisions, quadratic Bezier string vibrations, and scrolling musical staff notation.
3. **Single-File Architecture:**
   * HTML, CSS, and JavaScript are bundled cleanly into `index.html` for instant deployment and zero build steps.

---

## 🚀 How to Run Locally

1. Clone this repository:
   ```bash
   git clone [https://github.com/thisararukshan00-bit/kinetic-web-music-room.git](https://github.com/thisararukshan00-bit/kinetic-web-music-room.git)
