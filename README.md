# 🎮 STM32 Retro Handheld Console

A minimalist and low-cost DIY handheld game console powered by an STM32F103 ("Blue Pill"), featuring two classic games: **Snake** and **Pong**. Designed for portability, performance, and fun, this project showcases embedded systems skills from hardware to firmware.

---

## 📸 Preview

![console photo](./assets/console_photo.jpg)  
![gameplay gif](./assets/gameplay_snake.gif)

---

## 🧠 Features

- 🎮 Two games: **Snake** and **Pong**
- 🖥️ 1.8" TFT color display (ST7735, SPI)
- 🎛️ 6-button interface (D-pad, A, B, Start, Option)
- 🔉 Passive buzzer for game sounds
- 🔋 Rechargeable battery (Li-ion) with USB charging
- ⚙️ Coded in C using STM32 HAL libraries
- 🧩 Modular codebase (game engine, input, rendering)

---

## 🔩 Hardware Components

| Component | Description |
|----------|-------------|
| **MCU** | STM32F103C8T6 ("Blue Pill") |
| **Display** | 1.8" TFT LCD (ST7735, 128x160, SPI) |
| **Buttons** | 4 directional + A, B + Start, Option |
| **Audio** | Passive buzzer (GPIO + PWM) |
| **Battery** | 3.7V Li-ion + TP4056 charging module |
| **Others** | Pull-up resistors, perfboard or custom PCB, headers |

---

## 🧰 Project Structure

/stm32-handheld-console/
├── firmware/
│ ├── Core/
│ │ └── Src/ <- STM32 HAL source code
│ ├── games/
│ │ ├── snake.c
│ │ └── pong.c
│ ├── drivers/
│ │ └── st7735/
│ └── main.c
├── hardware/
│ ├── schematics.png
│ └── PCB_design.kicad_pcb
├── assets/
│ ├── console_photo.jpg
│ └── gameplay_snake.gif
└── README.md









---

## ⚙️ Software Tools

- **STM32CubeIDE** for development
- **ST-Link v2** programmer
- **KiCad** for PCB design (optional)
- **Fritzing** or hand-drawn schematics (early prototype)
- **PlatformIO** (alternative build system possible)

---

## 🚀 How to Build & Flash

1. Open `firmware/` with STM32CubeIDE
2. Select `BluePill` (STM32F103C8) as target board
3. Flash using ST-Link
4. Connect TFT (SPI) and buttons as per schematic
5. Power with 3.7V battery or USB via TP4056

---

## 🎯 Game Features

### 🐍 Snake
- Grid-based rendering on TFT
- Score tracking
- Speed increase with progression

### 🏓 Pong
- Player vs wall (or AI)
- Scoring + ball speed adjustment
- Smooth animation using DMA-friendly drawing

---

## 💡 Future Improvements

- Add SD card to store multiple games or assets
- Splash screen and game menu system
- Sound mixer with basic effects
- 3D-printed enclosure

---

## 🧑‍💻 Author

Designed and developed for educational purposes by an electronics engineering student.  
Feel free to fork, remix, or contribute!

---

## 📜 License

This project is licensed under the MIT License – see the [LICENSE](./LICENSE) file for details.


