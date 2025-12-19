# Kilo Text Editor

A feature-rich, lightweight text editor built from scratch in C. It runs purely in the terminal using standard POSIX libraries and VT100 escape sequences, requiring no external dependencies.

This project implements a complete TUI (Text User Interface) with advanced features like syntax highlighting, mouse tracking, and an internal clipboard.

## 🚀 Features

* **Syntax Highlighting:** Automatic highlighting for C/C++ files (keywords, strings, comments, numbers).
* **Line Numbering:** Professional gutter on the left displaying line numbers.
* **Mouse Support:** Click anywhere in the text to instantly move the cursor.
* **Search (`Ctrl+F`):** Incremental search with forward/backward navigation.
* **Clipboard:** Internal copy (`Ctrl+C`) and paste (`Ctrl+V`) support.
* **Raw Mode:** Custom terminal handling for a responsive, byte-level input experience.
* **Safe Quit:** "Dirty flag" protection warns you before quitting with unsaved changes.

## 🛠️ Tech Stack

* **Language:** C (C99 Standard)
* **System API:** POSIX (Portable Operating System Interface)
* **Input Handling:** `<termios.h>` for raw mode and mouse tracking.
* **Output Rendering:** VT100 / ANSI Escape Sequences.

## 📦 Installation & Build

### Prerequisites
You only need a C compiler (`gcc`) and `make`.
* **Linux/WSL:** `sudo apt install build-essential`
* **Mac:** `xcode-select --install`

### Build Instructions

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/yourusername/kilo-editor.git](https://github.com/yourusername/kilo-editor.git)
   cd kilo-editor

2. **Compile:**
   Run `make` to build the executable.
   ```bash
   make

3. **Run:**
    ./main [filename]
    