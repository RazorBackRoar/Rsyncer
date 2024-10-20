# TwinSync

TwinSync is a powerful, user-friendly folder synchronization and backup tool for macOS. It leverages the robust capabilities of rsync to ensure data integrity, preserve metadata, and offer advanced synchronization features.

## Table of Contents

1. [Overview](#overview)  
2. [Key Features](#key-features)  
3. [How It Works](#how-it-works)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Advanced Configuration](#advanced-configuration)  
7. [Troubleshooting](#troubleshooting)  
8. [Contributing](#contributing)  
9. [License](#license)  
10. [Contact](#contact)  

---

## Overview

TwinSync simplifies the process of keeping your important files and folders synchronized across multiple locations. Whether you're backing up critical data, maintaining dev/production parity, or keeping your work in sync across devices, TwinSync offers a reliable and efficient solution.

---

## Key Features

- **Intuitive Interface**: Drag-and-drop functionality for easy operation.  
- **Intelligent Synchronization**: Only transfers changed files to save time and bandwidth.  
- **Metadata Preservation**: Maintains file attributes, permissions, and timestamps.  
- **Flexible Scheduling**: Set up automatic syncs at specified intervals.  
- **Conflict Resolution**: Smart handling of conflicting changes with user-friendly options.  
- **Versioning**: Keeps multiple versions of changed files for easy recovery.  
- **Secure Transfer**: Option for encrypted transfers when syncing over networks.  
- **Cross-platform Compatibility**: Designed for macOS, with future Windows and Linux support planned.  
- **Detailed Logging**: Comprehensive logs for auditing and troubleshooting.  
- **Customizable Ignore Rules**: Easily exclude files or folders from syncing.  

---

## How It Works

1. **Source Selection**: Choose the folder you want to sync via drag-and-drop or file picker.  
2. **Destination Setup**: Select or create the destination for your synchronized data.  
3. **Configuration**: Set your preferences for sync behavior, scheduling, and conflict resolution.  
4. **Analysis**: TwinSync scans the source and destination, identifying differences.  
5. **Synchronization**: Files are copied, updated, or deleted based on your settings.  
6. **Verification**: A thorough check ensures data integrity post-sync.  
7. **Reporting**: Receive a detailed summary of the sync operation.  

---

## Installation

1. **Install Homebrew**:  
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install TwinSync**:  
   ```bash
   brew install twinsync
   ```

3. **Launch TwinSync**:  
   - From your **Applications** folder  
   - Or via command line:  
     ```bash
     twinsync
     ```

---

## Usage

### Basic Sync

1. Open TwinSync.  
2. Drag your source folder onto the TwinSync window.  
3. Select or create a destination folder.  
4. Click **“Sync Now.”**

### Command Line Usage

For advanced users, TwinSync can be operated via the command line:

```bash
twinsync sync /path/to/source /path/to/destination
```

---

## Advanced Configuration

Access advanced settings through the TwinSync preferences menu:

- **Sync Schedules**: Set up automatic syncs (hourly, daily, or weekly).  
- **Conflict Resolution**: Choose how to handle conflicting changes.  
- **Versioning**: Configure how many past versions of files to keep.  
- **Ignore Rules**: Set up patterns for files/folders to exclude.  
- **Network Settings**: Configure bandwidth limits and encryption for network syncs.  

---

## Troubleshooting

- **Sync Fails**: Ensure you have the necessary permissions for both source and destination.  
- **Slow Performance**: Check your network connection or try excluding large, frequently changing files.  
- **Conflicts**: Review the conflict resolution settings and manually resolve conflicts if needed.  

---

## Contributing

We welcome contributions to TwinSync! Here’s how you can help:

1. Fork the repository.  
2. Create a feature branch:  
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes:  
   ```bash
   git commit -m "Add some AmazingFeature"
   ```
4. Push to the branch:  
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a Pull Request.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and submission process.

---

## License

This project is licensed under the **MIT License**. See the [LICENSE.md](LICENSE.md) file for details.

---

## Contact

Your Name – [RazorBackRoar@icloud.com](mailto:RazorBackRoar@icloud.com)  
Project Link: [GitHub](https://github.com/RazorBackRoar/twinsync)
