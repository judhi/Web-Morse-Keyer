Demo page [https://judhi.github.io/Web-Morse-Keyer/morse_keyer.html]

# Web Morse Keyer v1.0

Welcome to **Web Morse Keyer v1.0**! This is a browser-based Morse code keyer that operates natively inside modern web browsers using pure HTML5, JavaScript, the **Web Audio API**, and the **Web Serial API**.

---

## 🎮 Input Sources

You can use any of these input options to key the application:

| Function | Keyboard | Serial I/O Port | Mouse Keying Area |
| :--- | :---: | :---: | :---: |
| **Left paddle (Dit)** | `[` | CTS | Left button |
| **Right paddle (Dah)** | `]` | DSR | Right button |

---

## ⌨️ Other Keyboard Shortcuts

| Key | Function |
| :---: | :--- |
| `\` | Straight key (Press & hold for continuous tone) |
| `-` | Decrease keyer speed (WPM) |
| `=` | Increase keyer speed (WPM) |
| `CTRL` + `ENTER` | Toggle TX (Text Transmission mode) |

---

## 🛠️ Features

- **Four Keying Modes:**
  - **Straight Key:** Manual keying input.
  - **Semi-Auto (Bug):** Generates automatic PARIS-timed dits while dahs remain manual.
  - **Iambic Paddles:** Supports both **Mode A** and **Mode B** (with a visual indicator for Mode B trailing element memory).
  - **Ultimatic Paddles:** Squeeze keying mode playing the most recently pressed lever.
- **Web Serial API Support:** Connect an external straight key, single-lever, or iambic paddle directly via serial hardware control lines (**CTS** and **DSR**).
- **Text Transmitter (TX):** Type or paste text into the TX input box to send automated Morse code at the configured WPM speed. Characters are automatically moved to the *Sent Text Output* display as they are sent.
- **Audio Output Routing:** Includes a master volume slider, envelope rise/fall shaping ($8\text{ ms}$ default to prevent audio clicks), and dynamic device selection via `setSinkId` to route audio to specific speakers, headphones, or Virtual Audio Cables (VAC).
- **Configuration Persistence:** Save and load configuration preferences via `serstat.cfg`.

---

## ⚡ Quick Start

1. Open the keyer in **Google Chrome**, **Microsoft Edge**, or **Opera** *(Firefox and Safari do not support the Web Serial API)*.
2. Click **Authorize Port** under the *Serial I/O* section if you are connecting physical paddles via a USB-to-Serial adapter.
3. Use the **Mouse Keying Area**, your keyboard (`[` and `]`), or serial hardware inputs to start keying!

---

## 🙏 Credits & Acknowledgments

This web application is inspired by the original **Morse Keyer** Windows app developed by **Robert B. Denny** ([rdenny@dc3.com](mailto:rdenny@dc3.com)).

**Created by:** *Judhi A65IV* ([judhi.a65iv@gmail.com](mailto:judhi.a65iv@gmail.com))
