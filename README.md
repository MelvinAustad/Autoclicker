# Universal AutoClicker

A cross-platform autoclicker with a modern, intuitive UI built with CustomTkinter. Supports Windows, macOS, and Linux.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-blue)

## Features

✨ **Intuitive UI** - Modern dark-themed interface with Catppuccin color palette  
⚡ **Fast Clicking** - Configurable click rates up to 200 CPS (0.01s interval)  
🎯 **Click Options** - Single, double, or triple click modes  
🖱️ **Mouse Buttons** - Support for left, right, and middle mouse buttons  
📍 **Fixed Position** - Click at a specific screen location  
⌨️ **Hotkey Recording** - Easy-to-use hotkey customization (F6 by default)  
⏱️ **Auto-Stop** - Automatic stopping after a set duration  
💾 **Config Persistence** - Settings saved between sessions  
🔄 **Cross-Platform** - Works on Windows, macOS, and Linux  

## Installation

### Prerequisites

- Python 3.8 or higher
- pip package manager

### Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/universal-autoclicker.git
cd universal-autoclicker
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python main.py
```

## Usage

### Basic Operation

1. **Set Click Rate** - Use the slider to adjust clicks per second (CPS) or enter a value manually
2. **Choose Click Type** - Select Single, Double, or Triple clicks
3. **Select Mouse Button** - Pick Left, Right, or Middle button
4. **Click Location** - Choose to click at current cursor or a fixed position
5. **Hotkey** - Default is F6; press "Record" to set a custom hotkey
6. **Start** - Click "Start Clicking" or press your hotkey

### Advanced Features

#### Fixed Position Clicking
- Select "Fixed" under "Click At"
- Press "Set" and wait for the countdown
- The position will be captured automatically

#### Configurable Click Rates
- Adjust via slider: 0.01s to 5.0s per click (10-200 CPS)
- Or enter CPS directly in the input field
- Values sync automatically

#### Auto-Stop
- Enable the auto-stop feature
- Set hours, minutes, and seconds
- Clicking will automatically stop after the duration
- Useful for grinding or batch operations

#### Hotkey Customization
- Click "Record" to enter recording mode
- Press any key within 5 seconds
- Your new hotkey is set immediately

## Configuration

Settings are automatically saved to:
- **Windows**: `C:\Users\[Username]\.config\universal-autoclicker\config.json`
- **macOS**: `/Users/[Username]/.config/universal-autoclicker/config.json`
- **Linux**: `/home/[Username]/.config/universal-autoclicker/config.json`

You can manually edit this JSON file or let the UI manage it.

## Troubleshooting

### Clicking doesn't work
- Check that you have the latest version: `pip install --upgrade -r requirements.txt`
- On macOS, you may need to grant accessibility permissions to your terminal/IDE
- On Linux, ensure you have the required permissions to access input devices

### Hotkey not responding
- Try a different key
- Some system hotkeys may be blocked
- Check the logs for errors

### UI scaling issues
- The app should auto-detect your display scaling
- If not, try adjusting your OS display settings

## System Permissions

### macOS
The application needs accessibility permissions to work:
1. Go to **System Preferences** → **Security & Privacy** → **Accessibility**
2. Add your Terminal/IDE to the allowed apps

### Linux
You may need to run with appropriate permissions:
```bash
sudo python main.py
```

Or configure udev rules for input device access.

### Windows
No special permissions required.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup
```bash
git clone https://github.com/yourusername/universal-autoclicker.git
cd universal-autoclicker
pip install -r requirements.txt
```

### Code Style
- Follow PEP 8 conventions
- Use type hints for all functions
- Add docstrings to all classes and functions
- Keep functions modular and well-documented

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This tool is provided for legitimate purposes only. The user is responsible for complying with all applicable laws and terms of service of any software they use this tool with. Unauthorized automation may violate terms of service or local laws. Use responsibly.

## Acknowledgments

- Built with [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter)
- Input handling with [pynput](https://github.com/moses-palmer/pynput)
- Color scheme inspired by [Catppuccin](https://catppuccin.com/)

## Support

If you encounter any issues, please:
1. Check the [troubleshooting section](#troubleshooting)
2. Review existing [issues](https://github.com/yourusername/universal-autoclicker/issues)
3. Create a new issue with detailed information about your problem
