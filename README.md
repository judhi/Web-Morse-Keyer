Demo page [https://judhi.github.io/Web-Morse-Keyer/morse_keyer.html]

# 📻 Web Morse Keyer v1.0

A lightweight, feature-rich browser-based Morse Code keyer and transmitter designed for amateur radio operators, CW practice, and field/QRP operations. Supports physical paddles via Web Serial, touch pads, keyboard keying, and multi-mode keyer logic.

---

## ✨ Features

- **Multiple Keyer Modes:**
  - **Iambic Paddles** (Mode A & Mode B with trailing memory)
  - **Semi-Automatic (Bug)**
  - **Ultimatic Paddles**
  - **Straight Key**
- **Flexible Hardware & Control Options:**
  - **Web Serial Interface:** Connect external physical paddles using serial control lines (**CTS** for Dit, **DSR** for Dah).
  - **Touch Interface:** Dedicated on-screen touch pads for mobile/tablet CW operation.
  - **Keyboard Keying:** Full keying support (`[` / `]` for paddles, `\` for straight key).
  - **Mouse Keying:** Integrated title bar keyer (Left-click = Dit, Right-click = Dah).
- **Text Transmitter (TX):**
  - Live text-to-CW transmission with real-time text character queueing.
  - **Shorthand Macros (F1–F5):** Quick-send macros for standard contest/QSO exchanges (`CQ`, `599`, `73`, etc.).
  - **3-Level Undo / Hold-to-Clear:** Tap to undo macro insertions (up to 3 levels) or long-press to clear unsent text.
- **Audio Engine:**
  - Customizable tone frequency (500 Hz – 1200 Hz) with adjustable rise/fall envelope time.
  - Multi-device audio routing (select custom soundcards or external audio interfaces).
- **Persistent Settings:** Automatically saves WPM, tone, volume, macros, and keyer modes to browser local storage.

---

## 🕹️ Input Controls & Shortcuts

### Keying Interfaces

| Function | Keyboard | Serial Port Line | Touch / Mouse |
| :--- | :--- | :--- | :--- |
| **Left Paddle (Dit)** | `[` | `CTS` | Title Bar Left-Click / Touch **"L"** |
| **Right Paddle (Dah)** | `]` | `DSR` | Title Bar Right-Click / Touch **"R"** |
| **Straight Key** | `\` | — | Middle Touch Pad **"S"** |

### Shortcuts & Shorthands

| Action | Control / Shortcut | Description |
| :--- | :--- | :--- |
| **Trigger Shorthand** | `F1` – `F5` | Inserts saved macro text into the TX queue. |
| **Configure Macros** | Long-Press `F1`–`F5` | Opens the configuration modal to edit shorthand texts. |
| **Undo Insertion** | Tap `Undo/Clear` | Undoes the last inserted F-key macro (up to 3 history levels). |
| **Clear Unsent Text** | Hold `Undo/Clear` | Clears all text from the unsent TX text box. |
| **Adjust Speed (WPM)** | `-` / `=` (or `_` / `+`) | Decreases or increases keying speed in WPM increments. |
| **Toggle TX** | `Ctrl + Enter` | Starts or stops automatic text transmission. |

---

## 🔌 Serial Port Hardware Hookup

To connect physical Morse paddles using an external USB-to-Serial adapter (e.g., FTDI, CH340, CP2102):

---

## 🙏 Credits & Acknowledgments

- **Inspiration:** Inspired by the original Morse Keyer Windows application developed by **Robert B. Denny** (`rdenny@dc3.com`).
- **Creator:** **Judhi A65IV** (`judhi.a65iv@gmail.com`)
- **AI Collaborator:** Developed in collaboration with **Gemini** (Google AI) as a vibe coding assistant for code architecture, UI refactoring, and mobile touch optimization.
