# 🎧 Hearing Loss & Hearing Aid Simulator – DE1-SoC Project

## 🎯 Purpose

This project simulates the experience of **hearing loss** and the effect of **hearing aids** using real-time audio processing, VGA visuals, and PS/2 keyboard inputs on the **DE1-SoC board**.

We created this to help raise awareness, foster empathy, and demonstrate the value of assistive technologies in hearing health. Through volume reduction, background noise distortion, and echo processing, users can "hear" what it might feel like to struggle with audio perception—and see how hearing aids might help.

---

## 🧠 What This Project Does

### 🔁 System Overview

- **Input**: Microphone or preloaded audio samples
- **Processing**:
  - Hearing Loss: Volume reduction, noise distortion, speech degradation
  - Hearing Aid: Volume gain, noise suppression, optional echo
  - Toggle echo, distortion, and low-pass filters
- **Output**: Processed stereo audio + VGA screen visuals
- **User Control**: PS/2 keyboard & DE1 keys for switching modes and levels

---

## 🖼 Block Diagram

![Block Diagram](https://github.com/hyeonjijung1/Hearing-Aid-Simulator/blob/main/Screenshot%202025-03-25%20020700.png?raw=true)

---

## 🖥 Screens & Modes

| Screen / Mode       | Description |
|---------------------|-------------|
| `Homepage`          | Intro screen; choose between samples or mic mode |
| `Mode Select`       | Pick sample 1 (conversation), 2 (busy street), 3 (orchestra), or mic input |
| `Simulator`         | Basic playback screen before choosing Aid/Loss |
| `Hearing Loss`      | Simulates muffled, distorted, or noisy hearing |
| `Hearing Aid`       | Adds gain, echo, and filters to enhance clarity |
| `Mic Mode`          | Real-time mic input with processing & echo options |

---

## 🎮 Controls (PS/2 Keyboard + Keys)

### 🔤 Keyboard Inputs

| Key         | Action |
|-------------|--------|
| `1`         | Select Sample 1 (Conversation) |
| `2`         | Select Sample 2 (Busy Street) |
| `3`         | Select Sample 3 (Orchestra) |
| `4`         | Switch to Microphone Input Mode |
| `←`         | Switch to Hearing Loss Simulator |
| `A`         | Switch to Hearing Aid Simulator |
| `V`         | Adjust Volume level |
| `N`         | Adjust Noise level |
| `S`         | Adjust Speech distortion level |
| `E`         | Toggle Echo (On/Off) |
| `H`         | Return to Homepage |
| `↑` / `↓`   | Increase / Decrease effect level |

---

## 🔊 Audio Features

### Hearing Loss Simulator:
- Volume reduction with multiple levels
- White noise overlay with adjustable intensity
- Speech distortion effects
- Optional low-pass filters
- Visual feedback via LED and screen

### Hearing Aid Simulator:
- Volume amplification (scaling)
- Noise subtraction
- Adjustable echo (damping constants)
- Real-time filtering (optional)
- Real-time distortion (clipping with gain)
- Bubble-like VGA visuals for gain levels

---

## 🎆 Visual Interface

- **VGA Display** shows UI transitions: Homepage, Mode Selector, Loss Simulator, Aid Simulator
- **LEDs** indicate current gain/noise mode and blink on max level
- **Pixel Drawing** for animated numeric visual gain levels

---

## 🧪 Try It Yourself (Emulator)

Try the project in-browser with this link:

🔗 [https://cpulator.01xz.net/?sys=rv32-de1soc](https://cpulator.01xz.net/?sys=rv32-de1soc)

### 🛠 Steps:
1. Change **language** to `C`
2. Upload `hearing_simulator.c` file
3. Open **PS/2 Keyboard 1** on the left panel
4. Interact using the controls above!

---

## 📁 File Structure

| File                  | Description |
|-----------------------|-------------|
| `hearing_simulator.c` | Main C file with audio & UI logic |
| `README.md`           | This file |
| `sample1[]`           | Conversation sample array (TODO: populate) |
| `sample2[]`           | Busy street sample array |
| `sample3[]`           | Orchestra sample array |
| `main_menu[]` etc.    | VGA image arrays for different screens |

---

## 👥 Team

- **Hyeonji Jung**
- **Shayana Ramachandran**

👨‍🎓 University of Toronto  
📚 ECE243 – Introduction to Computer Organization

---

## 💡 Future Improvements

- Add real waveform visualization on VGA
- Support recording and storing new user samples
- Add FFT-based frequency analysis
- Multi-language menu and audio prompts


