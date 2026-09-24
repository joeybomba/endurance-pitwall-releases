# Endurance Pitwall

**Free Windows pitwall and strategy software for iRacing endurance teams.**

Endurance Pitwall brings live race information, strategy, stint planning and team coordination together in one application.

**Endurance Pitwall is free and will stay free.** There is no subscription and no paid feature tier.

## What it does

- Live iRacing telemetry
- Fuel, pace and pit-window calculations
- Automatic and manually editable stint planning
- Multiple driver availability windows
- iRacing Fair Share checks
- Live track map and class standings
- Host, driver, crew and view-only access
- Pitwall calls, team notes and team chat
- Optional Garage61 analysis
- Race-plan PDF and Excel exports
- One-page post-race PDF report
- Responsive Display Mode for an extra monitor
- Four-driver Spa 24 Hours demo
- Custom application accent colours

## Download

Official releases are published here:

https://github.com/joeybomba/endurance-pitwall-releases/releases

Only download `Endurance Pitwall Setup.exe` from this repository.

## Windows SmartScreen / unsigned installer

The current Windows installer is **not digitally code-signed**.

Because of that, Microsoft SmartScreen may show an **Unknown publisher** or **Windows protected your PC** warning. That warning means Windows cannot verify the publisher identity through a trusted code-signing certificate. It is not, by itself, proof that malware was detected.

This project is still new, so users should make their own decision before running an unsigned executable.

## Transparency

This repository currently serves primarily as the **official release/download repository** for Endurance Pitwall.

The application source code and complete reproducible build workflow are **not yet published here**. We do not want the automatically generated GitHub “Source code” archives on a release page to be mistaken for proof that the installer was built from public source.

Improving release transparency is an active goal. Planned improvements include:

- Public build workflow
- Automated Windows builds
- SHA-256 checksums in release notes
- Build provenance / attestations where practical
- Better release documentation
- Digital code signing when practical

Until those are in place, please treat each release as an unsigned community-built Windows application and only download it from this repository.

## How Endurance Pitwall connects

### iRacing

Live telemetry is read locally from the running iRacing simulator through the iRacing SDK.

Endurance Pitwall does **not** need your iRacing account password to read local telemetry.

### Garage61

Garage61 integration is optional. If you enable it, you provide your own Garage61 API key for the features that use Garage61.

Never post your API key publicly in GitHub Issues, Discord messages, screenshots or logs.

### Team access

Host, driver, crew and view-only features can exchange race-related information between connected team members.

Only share host/view links or access codes with people you trust.

## Updates

Updates are never intentionally installed silently and are not intended to interrupt an active race.

Download new releases from the official Releases page.

## Verifying a file

Release notes may include a SHA-256 hash for the installer.

On Windows PowerShell you can calculate the hash of your downloaded installer with:

```powershell
Get-FileHash ".\Endurance Pitwall Setup.exe" -Algorithm SHA256
```

Compare the result with the SHA-256 value published with that release. If the values do not match, do not run the file.

## Screenshots

### Live Pitwall – Display Mode

![Endurance Pitwall Display Mode](Live%20demo.png)

### Live Pitwall – Main View

![Endurance Pitwall Main View](Live%20demo2.png)

### Race Planner – Overview

![Race Planner Overview](Stint%20Builder.png)

### Driver Availability & Stint Setup

![Driver Availability and Stint Setup](Stint%20Builder%202.png)

### Race Plan PDF Export

![Race Plan PDF Export](Pdf%20Export%20planning.png)

### Post-Race Report

![Post-Race Report](Post%20race.png)

## Security

Please read [SECURITY.md](SECURITY.md) before reporting a security-sensitive issue.

## Privacy

See [PRIVACY.md](PRIVACY.md) for a plain-language overview of the data and connections used by the application.

## Feedback and bug reports

Feedback, bug reports and feature suggestions are welcome.

When reporting a bug, please include:

- Endurance Pitwall version
- Windows version
- What you were doing when the issue occurred
- Whether iRacing was running
- Screenshots or error messages where useful

Do **not** include passwords, API keys or other secrets in public reports.

## Cost

Endurance Pitwall is free and is intended to remain free.

- No subscription
- No premium tier
- No features locked behind payment

## Disclaimer

Endurance Pitwall is an independent community project and is not affiliated with, sponsored by or endorsed by iRacing.com Motorsport Simulations.

Garage61 integration is optional. Endurance Pitwall is not affiliated with or endorsed by Garage61.
