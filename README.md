
```markdown
# 10 kHz Wien Bridge Oscillator with Sawtooth Waveform Conversion

This project involves designing and simulating a **10 kHz Wien Bridge Oscillator** and then converting the sinusoidal output into a **sawtooth waveform** with a rising time of approximately **90 microseconds**. The circuit was both simulated in **LTspice** and implemented on hardware as part of an Analog Electronics Lab group project at IIT Indore.

---

## 🧠 Project Overview

The circuit is built in multiple stages:
1. **Wien Bridge Oscillator** – generates a 10 kHz sine wave
2. **Inverting Amplifier** – reduces the amplitude to avoid saturation
3. **Comparator** – converts the sine wave to a 90% duty-cycle square wave
4. **Integrator** – converts the square wave into a sawtooth waveform

---

## 🔧 Tools & Components Used

### Simulation:
- Software: **LTspice XVII**
- Op-Amps: **LM741**
- Passive Components: Resistors, Capacitors

### Lab Implementation:
- Breadboard / Perfboard
- Function Generator (for testing)
- Oscilloscope (for waveform analysis)
- Power Supply: ±12V dual rail

---

## 🌀 Circuit Stages

### 1️⃣ Wien Bridge Oscillator
- Frequency formula:  
  \[
  f = \frac{1}{2\pi RC}
  \]
- Designed for 10 kHz with \( R = 10\,k\Omega \), \( C = 0.001\,\mu F \)
- Output: clean sine wave at ~10 kHz

### 2️⃣ Inverting Amplifier
- Used to reduce peak-to-peak voltage from ~14V to ~3V
- Gain = -R<sub>f</sub> / R<sub>in</sub>

### 3️⃣ Comparator
- Converts sine wave to square wave
- Set reference voltage to create 90% duty cycle

### 4️⃣ Integrator
- Converts square wave to sawtooth waveform
- Rise time tuned to ~90 µs using \( R = 100\,k\Omega \), \( C = 10\,nF \)

---

## 📷 Waveform Snapshots

| Stage         | Simulation Output |
|---------------|-------------------|
| Wien Oscillator | ![sine](./images/wien_output.png) |
| Comparator Output | ![square](./images/square_wave.png) |
| Sawtooth Output | ![sawtooth](./images/sawtooth_output.png) |

*(Replace with actual waveform images or screenshots from your LTspice and lab tests)*

---

## 📚 Learning Outcomes

- Designed stable low-distortion sine wave generators
- Understood waveform shaping using comparators and integrators
- Tuned circuits for precise timing and amplitude control
- Worked with both simulation and real-world op-amp limitations

---

## 🧑‍🤝‍🧑 Team Members

- Prateek Rajput (230002057)
- Kshithij Singhania (230002035)
- Anshita Pandey (230002010)
- Ayush Jindal (230002014)

---

## 📄 Report

[📎 Final Report (PDF)](https://drive.google.com/file/d/1NIJ04ShJh_91UKzQ97HiQF7xU8W8SBx_/view?usp=sharing)

---

## ✅ Status

- ✅ LTspice simulation completed and verified
- ✅ Lab implementation tested and waveforms validated

---

## 📁 Folder Structure

```

.
├── wien\_oscillator.asc           # LTspice file for sine wave
├── comparator.asc                # Square wave generator
├── integrator.asc                # Sawtooth generator
├── full\_circuit.asc              # Complete chain
├── images/
│   ├── wien\_output.png
│   ├── square\_wave.png
│   └── sawtooth\_output.png
└── README.md

```




---
