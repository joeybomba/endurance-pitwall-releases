# Endurance Pitwall 1.6.2

## Changes

- Removed the PayPal / support donation button from the application interface.
- Updated application and Windows installer version metadata to 1.6.2.
- No paid features or subscriptions were added.

## Build and verification

This release was built through the automated Windows build workflow using GitHub Actions.

Installer file:

`Endurance Pitwall Setup.exe`

SHA-256:

`2ca3275f8d90f35cc60d9ff4b4160a9c6eb7e5f2de61c0b56764f9bf74751694`

To verify the installer in PowerShell:

```powershell
Get-FileHash ".\Endurance Pitwall Setup.exe" -Algorithm SHA256
```

The calculated hash must match the value above.

## Windows SmartScreen

The installer is currently not digitally code-signed, so Microsoft SmartScreen may show an Unknown publisher warning.
