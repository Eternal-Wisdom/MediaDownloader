# MediaDownloader (v14.0.0)

Standalone, 100% lossless native Rust Windows desktop GUI & CLI media downloader.

## Features

- **100% Lossless Downloads**: Downloads original media files without re-encoding or quality loss.
- **8 Built-in Switchable Themes**:
  - Midnight Obsidian
  - Catppuccin Mocha
  - Tokyo Night
  - Rose Pine
  - Nord Frost
  - Dracula
  - OLED Pitch Black
  - Daylight Clean
- **Automatic Site Detection**: Supports 15+ websites with automatic URL and site detection.
- **4x Segmented Downloads & Resume**: Fast 4x segmented downloading with HTTP 206 partial-content resume support.
- **MD5 Checksum Verification**: Verifies downloaded files against server MD5 checksums to ensure integrity.
- **Native HLS (`.m3u8`) Support**: Built-in native HLS stream downloading without external tools.
- **Clipboard Monitor**: Automatically detects and queues supported URLs copied to the clipboard.
- **Persistent Queue**: Saves active and failed download queues (`r34_queue.json`, `r34_failed_queue.json`) across restarts.
- **SQLite WAL History DB**: Tracks download history in a fast SQLite WAL database (`r34_history.db`).
- **Optional JSON Sidecar Export**: Optionally exports metadata alongside downloaded media as JSON sidecar files.
- **HTTP / SOCKS5 Proxy Support**: Route downloads through HTTP or SOCKS5 proxies.
- **Windows Toast Notifications**: Native Windows desktop notifications for completed downloads and status updates.

## Quick Start

1. Download the latest release (`MediaDownloader_v14.0.0_Windows_x64.zip`) from the Releases page.
2. Extract the archive and run the executable to launch the desktop GUI (or invoke it via CLI).
3. Paste or copy a supported URL (with Clipboard Monitor enabled) and start downloading.

## Build from Source

Requires the Rust toolchain (`cargo` and `rustc`) on Windows:

```bash
# Run tests
cargo test

# Build optimized release binary
cargo build --release
```

## Privacy

All cookies, API keys, and user settings stay strictly local on your machine in `r34_config.json`. Nothing is transmitted to third-party servers., MD5 verification, persistent queue, and HLS support.
