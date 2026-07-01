# Bat File Editor

A standalone desktop IDE for editing Windows batch (.bat/.cmd) scripts, built with Python and Tkinter.

## Features

- **Real-time Syntax Highlighting**: Keywords, comments, variables, strings, labels, and numbers are highlighted with distinct colors
- **Command Reference Guide**: Interactive sidebar with searchable documentation for common batch commands (ECHO, SET, IF, GOTO, PAUSE, CHOICE, TIMEOUT, CLS, COLOR, TITLE, EXIT)
- **Simulated DOS Command Prompt**: Run batch scripts in a built-in simulator without leaving the application
- **Native CMD Execution**: Run scripts directly in Windows CMD (Windows only)
- **Gemini AI Copilot**: Integrated sidebar with AI assistance for code explanation, debugging, and optimization
- **Auto-backup**: Automatic backup of unsaved work every 60 seconds

## Installation

### From Source

```bash
pip install -r requirements.txt
python "batch file editor.py"
```

### Standalone Executable

Download the latest release from the `dist` folder:
- **Batch File Editor.exe** - One-file standalone executable
- **Bat File Explorer.exe** - Alternative build
- **Batch File Editor Updated/** - One-directory distribution

## Building from Source

```bash
pip install pyinstaller pillow
pyinstaller "Batch File Editor.spec"
```

The spec file includes the icon assets (`bat.png`, `bat_file_explorer.ico`, `bat_logo.png`).

## Usage

- **Ctrl+N**: New file
- **Ctrl+O**: Open file
- **Ctrl+S**: Save file
- **F1**: Help contents

## AI Copilot

1. Enter your Gemini API key in the AI Copilot tab
2. Use the buttons to:
   - Explain: Get a step-by-step explanation of your script
   - Check Errors: Analyze for bugs and security issues
   - Optimize: Get suggestions for cleaner, more modern code

## Project Structure

```
batch file editor/
├── batch file editor.py    # Main application
├── generate_icon.py        # Icon generator script
├── Batch File Editor.spec  # PyInstaller spec (one-file)
├── Bat File Explorer.spec  # Alternative spec
└── Batch File Editor Updated.spec  # One-directory spec
```

## Requirements

- Python 3.8+
- Tkinter (included with Python)
- PIL/Pillow (for icon handling)

## License

MIT License