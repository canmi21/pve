# PVZ Installer

This repository contains configurations and patches for running **Plants vs. Zombies** on Wine.

## Installation & Setup

### 1. Install Wine
Ensure you have Wine installed on your system. If not, install it using:

```sh
# Arch Linux
sudo pacman -S wine

# Debian/Ubuntu
sudo apt install wine
```

### 2. Configure Wine
Set up a **32-bit Wine prefix** to ensure compatibility:

```sh
WINEPREFIX=~/.wine WINEARCH=win32 winecfg
```

### 3. Run the Installer
Execute the installer using Wine:

```sh
wine pvz_installer.exe
```

## Patches & Fixes
- **3D Acceleration Fixes**: Enables better rendering support.
- **DDraw Rendering Fixes**: Improves performance and reduces graphical glitches.
- **DX12 Compatibility**: Enhances DirectX compatibility.

## Notes
- If you encounter graphical issues, try running `winecfg` and setting the graphics mode to **emulated virtual desktop**.
- Additional registry fixes can be found in the `configs/` directory.

## License
This repository only contains patches and configurations. The game itself is not included.


