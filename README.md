# Vortex RAT Builder

Vortex RAT Builder is a professional, open-source builder project for authorized device management, security research, and controlled lab testing. It combines a polished Windows builder UI with Telegram bot configuration, making it easier to configure, package, and manage authorized remote administration builds from one place.

**Official website:** [vortexcodes.org](https://vortexcodes.org)

> **Important:** Vortex RAT Builder must only be used for systems you own or have explicit permission to administer. Do not install, run, monitor, or collect data from any device without clear authorization.

## Project Status

- Fully open source for transparency, learning, review, and customization.
- Built around a Telegram bot workflow for authorized remote administration builds.
- Includes a modern Windows builder interface with setup, build, and support sections.
- Designed for authorized administrators, developers, and security researchers.

## Pricing

| Plan | Price | Includes |
| --- | ---: | --- |
| Lifetime Access | $30 one time | Project access, premium support, updates, and community access |
| Future Paid Updates | 30% off | Existing buyers receive a 30% discount on future paid upgrade packages or premium add-ons |

The source is open for review and learning. The paid lifetime option supports active development, support, packaged releases, and future maintenance.

## Buy And Support

To buy Vortex RAT Builder or request support:

- Direct message: [t.me/highoncodes](https://t.me/highoncodes)
- Support and update channel: [t.me/VortexPremiumRat](https://t.me/VortexPremiumRat)
- Website: [vortexcodes.org](https://vortexcodes.org)

## Screenshots

The screenshots below show the main Vortex RAT Builder workflow: setup guidance, build configuration, packaging progress, and build completion.

### Builder Configuration

![Vortex RAT Builder credentials and customization screen](screenshots/photo_2026-06-12_12-09-31.jpg)

The Builder tab is where users enter their Telegram bot token, admin user ID, executable name, optional icon, and administrator prompt preference before packaging a build.

### Setup Guide

![Vortex RAT Builder setup guide screen](screenshots/photo_2026-06-12_12-09-45.jpg)

The Setup Guide explains the first-time configuration flow, including creating a Telegram bot, saving the bot token, and finding the admin Telegram user ID used for access control.

### Build Progress

![Vortex RAT Builder build progress screen](screenshots/photo_2026-06-12_12-10-05.jpg)

The build screen shows the selected executable name, optional administrator prompt setting, dependency checks, and packaging progress while the builder prepares the output.

### Build Complete

![Vortex RAT Builder success dialog](screenshots/photo_2026-06-12_12-10-12.jpg)

After a successful build, Vortex RAT Builder shows the output executable path and reminds the user to connect through the configured Telegram bot.

### Telegram Status Updates

![Vortex RAT Builder Telegram connection status](screenshots/photo_2026-06-12_12-09-50.jpg)

When an authorized build connects, the configured Telegram admin receives a status card with device context such as user, host, OS, admin state, IP details, and uptime.

## Core Features

### Telegram-Based Control

Vortex RAT Builder configures builds that use Telegram as the command and notification layer. Authorized admins can manage connected devices, receive startup notifications, switch between active sessions, and keep track of online machines through a simple chat-based workflow.

Highlights:

- Admin-only access control using a configured Telegram user ID.
- Multi-device session handling.
- Device registration and online status tracking.
- Session switching for managing several authorized machines.
- Startup notification when an authorized device comes online.

### Modern Builder UI

The included builder provides a clean desktop interface for preparing Vortex RAT Builder builds without manually editing configuration values.

Highlights:

- Midnight-style dark interface.
- Setup guide, builder, and support pages.
- Telegram bot token and admin ID configuration.
- Custom executable name support.
- Optional custom Windows icon support.
- Optional administrator privilege request during build.
- Dependency checks before packaging.
- PyInstaller-based standalone executable creation.
- Built-in Telegram support buttons.

### System Administration

Vortex RAT Builder packages a broad set of system management tools for authorized Windows administration.

Highlights:

- Full system information reporting.
- Admin/elevation status checks.
- Current user and date/time information.
- CPU, RAM, OS, uptime, and hardware overview.
- Process listing and process termination.
- Installed software inventory.
- Windows service listing.
- Idle time reporting.
- Lock, sleep, shutdown, restart, and logoff actions.
- Startup persistence management.

### File Management

The file management module helps administrators inspect, organize, and transfer files on authorized devices.

Highlights:

- View and change the current working directory.
- List folder contents.
- Show mounted drives.
- Search for files by name.
- Upload and download files.
- Download files from a URL to the authorized device.
- Copy, move, rename, delete, and open files.
- Create folders.
- Encrypt and decrypt files with a provided key.

### User Interaction Tools

Vortex RAT Builder can package tools for visible interaction with an authorized device during support, testing, or demonstration sessions.

Highlights:

- Display message dialogs.
- Show custom error dialogs.
- Use text-to-speech output.
- Type provided text into the active session.
- Open websites in the default browser.
- Change the desktop wallpaper.
- Play audio files.
- Control volume and mute state.
- Turn monitors off.
- Hide or show the taskbar and desktop icons.
- Swap and restore mouse button behavior.

### Capture And Monitoring

For consent-based support, diagnostics, and lab testing, Vortex RAT Builder can package capture and monitoring utilities.

Highlights:

- Capture screenshots.
- Read and set clipboard text.
- List connected cameras.
- Select a camera index.
- Capture webcam images.
- Record microphone audio for a chosen duration.
- Start and stop keyboard activity logging for authorized audit sessions.

These features handle sensitive user information and should only be used with clear consent.

### Security Audit And Recovery Modules

Vortex RAT Builder includes optional data-audit modules intended for controlled environments, account recovery testing, and authorized security review.

Highlights:

- Browser credential audit support.
- Cookie/session inventory support (single site or all cookies).
- Public IP and geolocation lookup.
- Discord token audit support.
- Roblox account/session audit support.
- Steam account/session audit support.
- Environment variable listing.

Only use these modules on accounts, browsers, and devices you own or are explicitly authorized to inspect.

### Network Utilities

The network module helps inspect connectivity and local Windows network state.

Highlights:

- Nearby Wi-Fi network listing.
- Saved Wi-Fi profile review (credentials).
- Local IP configuration output.
- Active connection listing.
- Hosts-file based site block and unblock support.

### Advanced Windows Controls

Vortex RAT Builder also includes advanced Windows control features for lab testing and administrator-controlled environments.

Highlights:

- Startup entry management.
- Task Manager enable/disable controls.
- Windows Defender enable/disable controls.
- Windows Firewall enable/disable controls.
- Controlled blue screen test action.
- Critical-process test mode.
- Device registry reset for Vortex session tracking.

These options can affect system stability and security. Use them only in isolated labs or on machines where you have permission and a recovery plan.

## Project Files

| File | Purpose |
| --- | --- |
| `builder.py` | Desktop builder UI for configuring and packaging Vortex RAT Builder builds. |
| `client.py` | Build template/client logic and Telegram command handler. |
| `requirements.txt` | Python dependencies used by the builder and client. |
| `icon.ico` | Default Windows icon used by the project. |

## Requirements

- Windows environment for full feature support.
- Python 3.8 or newer.
- Telegram bot token.
- Telegram admin user ID.
- Dependencies listed in `requirements.txt`.

Install dependencies:

```bash
pip install -r requirements.txt
