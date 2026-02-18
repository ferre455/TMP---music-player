# TMP — Music Player

TMP is a minimal, interactive terminal-based music player written in Python. It leverages `mpv` for high-quality audio playback and provides a clean interface for your local music collection.

---

## 🛠 Features
* **Interactive Album Art**: Displays cover art in a dedicated window that stays on top of your work.
* **Terminal-First Design**: Full control via keyboard shortcuts without leaving your terminal.
* **Dynamic Navigation**: Smooth scrolling through your music directory with a persistent selection cursor.
* **Smart Auto-Next**: Automatically plays the next song with a safety guard to prevent accidental skipping.

---

## 📥 Installation & Dependencies

TMP requires **Python 3** and **mpv**. Follow the instructions for your operating system:

### 1. Install System Dependencies

#### **Linux**
* **Arch Linux:** `sudo pacman -S mpv`
* **Debian / Ubuntu / Mint:** `sudo apt update && sudo apt install mpv`
* **Fedora:** `sudo dnf install mpv`

#### **macOS**
Using [Homebrew](https://brew.sh/):
```sh
brew install mpv

```

#### **Windows**

1. Download the `mpv` bootstrap from [mpv.io](https://mpv.io/installation/).
2. Extract it to a folder (e.g., `C:\mpv`).
3. Add that folder to your System **PATH** so the script can find the `mpv` command.

---

### 2. Download and Run TMP

Clone the repository:

```sh
git clone [https://github.com/ferre455/TMP---music-player.git](https://github.com/ferre455/TMP---music-player.git)
cd TMP---music-player

```

Run the player:

```sh
python3 tmp.py

```

---

## 🎮 Controls & Navigation

TMP uses intuitive keyboard shortcuts to keep you in control of your music.

### **Navigation**

* **↑ / ↓ (Arrow Keys)**: Move the selector up or down the list.
* **Enter**: Play the currently selected song.
* **← / → (Left/Right)**: Instantly skip to the **Previous** or **Next** song in the list.

### **Playback Control**

* **Space**: Pause or Resume playback.
* **s**: **Shuffle** your music list (re-randomizes the order).
* **+ / -**: Increase or decrease **Volume**.
* **q**: Quit the player and close all windows.

---

## 📝 Important Notes

* **Music Location**: By default, TMP looks for music in your `~/Music` folder.
* **Supported Formats**: Supports `.mp3`, `.wav`, `.flac`, `.ogg`, and `.m4a`.
* **Window Focus**: The album art window is set to "Always on Top" (`--ontop`) but remains interactive.
* **Stability**: The script includes a confirmation logic (debounce) when starting songs to ensure smooth transitions.

```

```
