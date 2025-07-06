# 10 kHz Wien Bridge Oscillator with Sawtooth Waveform Conversion

This project involves designing and simulating a **10 kHz Wien Bridge Oscillator**, followed by the conversion of its sinusoidal output into a **sawtooth waveform** with a rising time of approximately **90 microseconds**. The circuit was simulated in **LTspice** and also implemented on hardware as part of the Analog Electronics Lab group project at **IIT Indore**.

---

## 🧠 Project Overview

The circuit consists of the following stages:

1. **Wien Bridge Oscillator** – Generates a 10 kHz sine wave  
2. **Inverting Amplifier** – Reduces amplitude to prevent saturation  
3. **Comparator** – Converts the sine wave to a square wave with ~90% duty cycle  
4. **Integrator** – Converts the square wave to a sawtooth waveform  

---

## 🔧 Tools & Components Used

### Simulation
- **Software**: LTspice XVII  
- **Op-Amps**: LM741  
- **Passive Components**: Resistors and capacitors  

### Hardware Implementation
- Breadboard / Perfboard  
- Function Generator (for testing)  
- Oscilloscope (for waveform observation)  
- Dual Power Supply: ±12V  

---

## 🌀 Circuit Stages

### 1️⃣ Wien Bridge Oscillator
- Frequency formula:  
  \[
  f = \frac{1}{2\pi RC}
  \]
- Designed for 10 kHz using:  
  \( R = 10\,k\Omega \), \( C = 0.001\,\mu F \)  
- Output: clean sine wave at ~10 kHz  

### 2️⃣ Inverting Amplifier
- Used to reduce the peak-to-peak voltage from ~14V to ~3V  
- Gain:  
  \[
  \text{Gain} = -\frac{R_f}{R_{in}}
  \]

### 3️⃣ Comparator
- Converts sine wave to square wave  
- Reference voltage is tuned to achieve ~90% duty cycle  

### 4️⃣ Integrator
- Converts square wave into a sawtooth waveform  
- Rise time adjusted to ~90 µs using:  
  \( R = 100\,k\Omega \), \( C = 10\,nF \)

---

## 📷 Waveform Snapshots

| Stage               | Simulation Output                     |
|---------------------|----------------------------------------|
| Wien Oscillator     | ![Sine Wave](./images/wien_output.png) |
| Comparator Output   | ![Square Wave](./images/square_wave.png) |
| Sawtooth Output     | ![Sawtooth](./images/sawtooth_output.png) |

> *(Replace with actual waveform images from LTspice/lab experiments)*

---

## 📚 Learning Outcomes

- Designed stable, low-distortion sine wave generators  
- Understood waveform shaping using comparators and integrators  
- Tuned analog circuits for precise timing and amplitude control  
- Gained hands-on experience with real-world op-amp limitations in lab settings  

---

## 🧑‍🤝‍🧑 Team Members

- Prateek Rajput (230002057)  
- Kshithij Singhania (230002035)  
- Anshita Pandey (230002010)  
- Ayush Jindal (230002014)  

---

## 📄 Project Report

📎 [Final Report (PDF)](https://drive.google.com/file/d/1NIJ04ShJh_91UKzQ97HiQF7xU8W8SBx_/view?usp=sharing)

---

## ✅ Project Status

- ✅ Simulation completed and verified in LTspice  
- ✅ Lab implementation tested and waveform output validated  

---
