# HomeKam releases

HomeKam is a home camera monitor for Windows. It runs on your PC: detection, recording and face matching happen locally, and HomeKam sends nothing off the computer unless you turn on email alerts. The desktop window uses Microsoft Edge WebView2, whose required diagnostic data follows your Windows Diagnostic data setting.

This repository only hosts installers. Download the latest one from [Releases](https://github.com/krislovescalifornia/HomeKam-releases/releases/latest).

## Install

1. Download `HomeKam-<version>-Windows-x64-Setup.exe` and `SHA256SUMS.txt` from the same release.
2. Check the installer in PowerShell:

   ```powershell
   (Get-FileHash .\HomeKam-<version>-Windows-x64-Setup.exe -Algorithm SHA256).Hash
   ```

   The result must match the line in `SHA256SUMS.txt`. If it doesn't, delete the file and don't run it.
3. Run the installer. It installs for your account only and needs no administrator rights.

Requirements: Windows 10 or 11 (x64), and Microsoft Edge WebView2 (included with current Windows).

## Unsigned builds

The installers are not code-signed yet, so Windows SmartScreen shows "Windows protected your PC" with "Unknown publisher". Choose **More info › Run anyway** only after the checksum above matches. Signing is planned for a later release.

## Preview status

These are development previews tested with generated video, not a finished product. Upgrading keeps your configuration and recordings.
