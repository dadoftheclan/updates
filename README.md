# 🚀 Enhanced Visual Windows Update Script

A visually stunning PowerShell script for managing Windows Updates in non-GUI environments with beautiful progress bars, colorful status displays, and comprehensive logging.

## ✨ Features

- **🎨 Enhanced Visual Interface** - Beautiful ASCII art banners, animated progress bars, and colorful status displays
- **📊 Comprehensive Reporting** - Detailed tables showing available updates with size, type, and KB article information
- **🔄 Multiple Update Categories** - Support for All, Software, Driver, and Optional updates
- **💾 Data Export** - Automatic export to CSV, JSON, and detailed log files
- **🤖 Silent Mode** - Fully automated operation for scripting scenarios
- **🛡️ Safe Operations** - Built-in validation and error handling
- **📋 Interactive Selection** - Choose specific updates or install all available
- **🔄 Reboot Management** - Intelligent restart handling with user confirmation

## 🎯 Use Cases

- **Headless Servers** - Perfect for server environments without GUI
- **Automation Scripts** - Silent mode for scheduled maintenance
- **Audit & Compliance** - Detailed logging and reporting for compliance requirements
- **Selective Updates** - Choose exactly which updates to install
- **Visual Feedback** - Beautiful progress indication for long-running operations

## 📋 Prerequisites

- **Windows PowerShell 5.1** or newer
- **Administrator privileges** required
- **Windows Update service** must be running
- **Internet connectivity** for downloading updates

## 🚀 Quick Start

### Basic Usage

```powershell
# Run interactively with visual interface
.\Updates.ps1

# Install all available updates silently
.\Updates.ps1 -All -Silent

# Install only software updates
.\Updates.ps1 -Software

# Install driver updates without reboot
.\Updates.ps1 -Driver -NoRestart
```

### Advanced Examples

```powershell
# Silent installation of optional updates only
.\Updates.ps1 -Optional -Silent -NoRestart

# Interactive mode for software updates with logging
.\Updates.ps1 -Software
```

## 🛠️ Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| `-All` | Switch | Install all available updates |
| `-Software` | Switch | Install software updates only |
| `-Driver` | Switch | Install driver updates only |
| `-Optional` | Switch | Install optional updates only |
| `-Silent` | Switch | Run without user interaction |
| `-NoRestart` | Switch | Suppress automatic reboot |

## 📊 Output Files

The script automatically generates several output files in the script directory:

- **`UpdateList.csv`** - Tabular data of all available updates
- **`UpdateList.json`** - Structured JSON data for programmatic use
- **`UpdateLog.txt`** - Detailed execution log with timestamps

## 🎨 Visual Features

### Animated Banner
```
██╗    ██╗██╗███╗   ██╗██████╗  ██████╗ ██╗    ██╗███████╗
██║    ██║██║████╗  ██║██╔══██╗██╔═══██╗██║    ██║██╔════╝
██║ █╗ ██║██║██╔██╗ ██║██║  ██║██║   ██║██║ █╗ ██║███████╗
[*] ENHANCED VISUAL EDITION v2.0 [*]
```

### Progress Indicators
- **Spinning loaders** for search operations
- **Progress bars** for downloads and installations
- **Color-coded status** for success/failure indication
- **Structured tables** for update information

### Status Boxes
```
+---------------------------------------+
| [+] SUCCESS!                          |
|                                       |
| All updates installed successfully!   |
+---------------------------------------+
```

## 📝 Example Session

```powershell
PS C:\Scripts> .\Updates.ps1 -Software

# Animated banner displays
# Scanning for software updates...
# Update table shows available updates
# Interactive menu for selection
# Progress bars during download/install
# Final summary report
```

## 🔧 Error Handling

The script includes comprehensive error handling for:

- **Network connectivity issues**
- **Windows Update service problems**
- **Insufficient permissions**
- **Download failures**
- **Installation errors**

All errors are logged with timestamps and detailed error messages.

## 📊 Update Categories

### Software Updates
- Security updates
- Critical updates
- Feature updates
- Quality updates

### Driver Updates
- Hardware driver updates
- Firmware updates
- Device-specific updates

### Optional Updates
- Language packs
- Feature updates
- Non-critical improvements

## 🔄 Reboot Handling

The script intelligently handles system reboots:

- **Automatic detection** of reboot requirements
- **User confirmation** in interactive mode
- **Countdown timer** in silent mode
- **Override option** with `-NoRestart` parameter

## 📋 Logging

Detailed logging includes:

- **Execution timestamps**
- **Update search results**
- **Installation outcomes**
- **Reboot requirements**
- **User selections**
- **Error messages**

## 🛡️ Security Considerations

- **Always run as Administrator** for proper Windows Update access
- **Review updates** before installation in production environments
- **Test in development** environments first
- **Backup critical systems** before major updates
- **Monitor logs** for any installation issues

## 🤝 Contributing

Contributions are welcome! Please feel free to submit:

- **Bug reports** with detailed error information
- **Feature requests** for new functionality
- **Pull requests** with improvements
- **Documentation updates**

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Authors

- **DadOfTheClan** - Original concept and implementation

## 🙏 Acknowledgments

- Microsoft Windows Update API documentation
- PowerShell community best practices
- ASCII art generation tools
- Community feedback and testing

## 🔗 Related Projects

- [PSWindowsUpdate](https://github.com/mgajda83/PSWindowsUpdate) - Alternative PowerShell module
- [Windows Update MiniTool](https://www.wilderssecurity.com/threads/windows-update-minitool.408842/) - GUI alternative
- [WSUS Offline Update](http://www.wsusoffline.net/) - Offline update solution

---

**⭐ If this script helped you, please consider giving it a star!**

**🐛 Found a bug? Please report it in the Issues section.**

**💡 Have an idea? We'd love to hear about it!**
