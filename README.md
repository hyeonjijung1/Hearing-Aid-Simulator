# Hearing Loss & Hearing Aid Simulator – DE1-SoC Project

## 🧠 Project Purpose

We created this project because we care about people who live with hearing difficulties. Our goal is to help others understand what it feels like to experience hearing loss and how hearing aids can make a difference.

By using the DE1-SoC board, we built a simulator that shows how hearing can change when volume is reduced or when background noise becomes hard to ignore. We also show how hearing aids can help by making sounds louder and clearer.

This project is made with kindness and a hope to build more awareness, empathy, and appreciation for assistive technologies that help people hear better.

---
## 🔧 What This Project Does

- **VGA Display Interface**  
  Shows different screens (homepage, hearing loss mode, hearing aid mode, etc.) using pixel plotting.

- **PS/2 Keyboard Input**  
  Lets users switch between modes (`v`, `n`, `r`, `d`), replay audio, and adjust gain using keyboard keys.

- **Audio Output Simulation**  
  Plays audio with effects that include:
  - **Volume reduction** (to show hearing loss)
  - **Noise distortion** (to simulate noisy environments)
  - **Volume and noise gain** (to simulate hearing aid help)

- **LED Feedback System**  
  Lights up to show the level of gain and blinks when the highest level is reached.

---
## 🧪 Try It Yourself (Anyone Can!)

Anyone can try our simulator online using the DE1-SoC emulator:

🔗 **Go to:** [https://cpulator.01xz.net/?sys=rv32-de1soc](https://cpulator.01xz.net/?sys=rv32-de1soc)

### Instructions:
1. Change the language to **C** using the dropdown.
2. Upload our `.c` file to the editor.
3. Click **PS/2 Keyboard 1** on the side panel to open the virtual keyboard.
4. Use the following keys:
   - `A` → Go to **Hearing Aid** simulator
   - `L` → Go to **Hearing Loss** simulator
   - `V` → Switch to **volume gain** control
   - `N` → Switch to **noise gain** control
   - `R` → Enter **volume reduction** mode (Loss)
   - `D` → Enter **distortion** mode (Loss)
   - `KEY0` (on emulator) → Increase gain level
   - `KEY1` → Reset gain levels
   - `KEY3` → Replay the audio

---


## 📊 Block Diagram

> 🖼️ Insert your system block diagram image here (e.g., `block_diagram.png`)  

