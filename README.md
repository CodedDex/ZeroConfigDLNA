# ZeroConfigDLNA 📺

Welcome to the **ZeroConfigDLNA** repository! This project allows you to stream media to your TV with just one command. Enjoy a seamless experience in your home theater setup without the need for complex configurations.

![ZeroConfigDLNA](https://img.shields.io/badge/Download-Release-blue?style=flat&logo=github&link=https://github.com/CodedDex/ZeroConfigDLNA/releases)

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Supported Formats](#supported-formats)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Easy Setup**: Stream media to your TV with a single command.
- **Supports Multiple Formats**: Play MKV, MP4, and more.
- **Cross-Platform**: Works on Windows, macOS, and Linux.
- **Integration with VLC**: Leverage VLC's powerful media capabilities.
- **Lightweight**: Minimal resource usage for smooth performance.

## Installation

To get started, you need to download the latest release. Visit the [Releases section](https://github.com/CodedDex/ZeroConfigDLNA/releases) to find the appropriate file for your operating system. Download and execute the file to install ZeroConfigDLNA.

### Prerequisites

- Python 3.x
- FFmpeg
- A compatible media player (VLC recommended)

### Step-by-Step Guide

1. **Download**: Go to the [Releases section](https://github.com/CodedDex/ZeroConfigDLNA/releases) and download the file for your OS.
2. **Install Dependencies**: Make sure you have Python and FFmpeg installed. You can install FFmpeg via your package manager or download it from the official website.
3. **Run the Script**: Open your terminal or command prompt, navigate to the directory where you installed ZeroConfigDLNA, and run the command:

   ```bash
   python zero_config_dlna.py
   ```

4. **Follow Prompts**: The script will guide you through the setup process.

## Usage

Using ZeroConfigDLNA is straightforward. After installation, you can stream media to your TV by executing the command:

```bash
python zero_config_dlna.py --media <path_to_your_media_file>
```

Replace `<path_to_your_media_file>` with the actual path of the media you want to stream. The script will automatically detect your DLNA-compatible devices on the network.

### Example

To stream a video file located at `/home/user/videos/sample.mp4`, you would run:

```bash
python zero_config_dlna.py --media /home/user/videos/sample.mp4
```

Your media will start playing on the selected device.

## Supported Formats

ZeroConfigDLNA supports a variety of media formats, including:

- **Video Formats**: MKV, MP4, AVI, MOV
- **Audio Formats**: MP3, AAC, WAV, FLAC

Check your media player documentation for a complete list of supported formats.

## How It Works

ZeroConfigDLNA uses the Universal Plug and Play (UPnP) protocol to discover and interact with DLNA devices on your network. The script sends commands to the media player, allowing you to control playback directly from your terminal.

### Architecture Overview

1. **Discovery**: The script scans the local network for DLNA devices.
2. **Playback Control**: It communicates with the media player to start, pause, or stop playback.
3. **Transcoding**: FFmpeg is used for on-the-fly transcoding, ensuring compatibility with various formats.

### Example Workflow

1. Start the script.
2. The script finds available devices.
3. You select a device.
4. You specify the media file.
5. The media plays on your selected device.

## Contributing

We welcome contributions to ZeroConfigDLNA! If you have ideas for new features, improvements, or bug fixes, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request.

Please ensure your code adheres to the project's coding standards and includes appropriate tests.

## License

ZeroConfigDLNA is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions or support, feel free to reach out:

- **Email**: support@zeroconfigdlna.com
- **GitHub**: [CodedDex](https://github.com/CodedDex)

Thank you for checking out ZeroConfigDLNA! We hope you enjoy streaming your media effortlessly.