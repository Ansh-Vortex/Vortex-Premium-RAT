# Vortex Advanced Remote Administration Tool

Vortex is a professional, open-source remote administration project built for authorized device management, security research, and controlled lab testing. It combines a Telegram-based control workflow with a polished Windows builder UI, making it easier to configure, package, and manage remote administration agents from one place.

Official website: [vortexcodes.org](https://vortexcodes.org)

> Important: Vortex must only be used on systems you own or have explicit permission to administer. Do not install, run, monitor, or collect data from any device without clear authorization.

## Project Status

- Fully open source for transparency, learning, review, and customization.
- Built around a Telegram bot workflow for fast remote administration.
- Includes a modern Windows builder interface with setup, build, and support sections.
- Designed for authorized administrators, developers, and security researchers.

## Pricing

| Plan | Price | Includes |
| --- | ---: | --- |
| Lifetime Access | $30 one time | Project access, premium support, updates, and community access |
| Future Paid Updates | 30% off | Existing buyers receive a 30% discount on future paid upgrade packages or premium add-ons |

The source is open for review and learning. The paid lifetime option supports active development, support, packaged releases, and future maintenance.

## Buy And Support

To buy Vortex or request support:

- Direct message: [t.me/highoncodes](https://t.me/highoncodes)
- Support and update channel: [t.me/VortexPremiumRat](https://t.me/VortexPremiumRat)
- Website: [vortexcodes.org](https://vortexcodes.org)

## Core Features

### Telegram-Based Control

Vortex uses Telegram as the command and notification layer. Authorized admins can manage connected devices, receive startup notifications, switch between active sessions, and keep track of online machines through a simple chat-based workflow.

Highlights:

- Admin-only access control using a configured Telegram user ID.
- Multi-device session handling.
- Device registration and online status tracking.
- Session switching for managing several authorized machines.
- Startup notification when an authorized device comes online.

### Modern Builder UI

The included builder provides a clean desktop interface for preparing Vortex builds without manually editing configuration values.

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

Vortex includes a broad set of system management tools for authorized Windows administration.

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

Vortex provides tools for visible interaction with an authorized device during support, testing, or demonstration sessions.

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

For consent-based support, diagnostics, and lab testing, Vortex includes capture and monitoring utilities.

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

Vortex includes data-audit modules intended for controlled environments, account recovery testing, and authorized security review.

Highlights:

- Browser credential audit support.
- Cookie/session inventory support.
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
- Saved Wi-Fi profile review.
- Local IP configuration output.
- Active connection listing.
- Hosts-file based site block and unblock support.

### Advanced Windows Controls

Vortex also includes advanced Windows control features for lab testing and administrator-controlled environments.

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
| `builder.py` | Desktop builder UI for configuring and packaging Vortex. |
| `client.py` | Main remote administration agent and Telegram command handler. |
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
```

Run the builder:

```bash
python builder.py
```

## Responsible Use

Vortex is a powerful administration framework. By using it, you agree to the following rules:

- Use it only on devices you own or have explicit permission to manage.
- Do not use it for unauthorized access, surveillance, credential theft, harassment, or evasion.
- Do not deploy it silently or deceptively.
- Tell users what is being installed, what it can access, and how it can be removed.
- Follow all laws and platform rules in your country or region.

The author and contributors are not responsible for misuse, damage, illegal activity, or policy violations caused by this software.

## Support

For help, updates, custom requests, or purchase questions:

- DM: [t.me/highoncodes](https://t.me/highoncodes)
- Channel: [t.me/VortexPremiumRat](https://t.me/VortexPremiumRat)
- Website: [vortexcodes.org](https://vortexcodes.org)

Thank you for supporting Vortex and the Vortex Codes community.
