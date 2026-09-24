# Security Policy

## Official downloads

Only download Endurance Pitwall from the official GitHub Releases page:

https://github.com/joeybomba/endurance-pitwall-releases/releases

Do not treat installers uploaded to third-party websites, mirrors or file-sharing services as official releases.

## Current signing status

Current Windows installers may be unsigned.

As a result, Microsoft SmartScreen may report **Unknown publisher** or display a warning before launch. This means Windows cannot verify the publisher identity through a trusted code-signing certificate.

An unsigned installer should be treated with appropriate caution.

## Release verification

Where a release includes a SHA-256 checksum, you can verify the downloaded installer in PowerShell:

```powershell
Get-FileHash ".\Endurance Pitwall Setup.exe" -Algorithm SHA256
```

The result must exactly match the checksum published in the release notes.

A matching checksum verifies that your downloaded file matches the file for which that checksum was published. It does **not** by itself prove that the application is free of vulnerabilities or malicious code.

## Credentials and secrets

Endurance Pitwall does not need your iRacing account password to read local telemetry.

Optional integrations may use API keys, such as Garage61.

Never post passwords, API keys, access codes or other secrets in public GitHub Issues, Discord channels, screenshots or logs.

If you accidentally expose an API key, revoke or rotate it with the relevant service.

## Reporting a security issue

For ordinary bugs, please use GitHub Issues.

For a security-sensitive problem, avoid publishing exploit details or secrets in a public issue. Examples include:

- Exposure of API keys
- Authentication or access bypass
- Unexpected remote access
- Arbitrary file access
- Remote code execution
- Unsafe update behavior
- Executable tampering
- Unexpected transmission of private data

Please contact the project owner through GitHub first so the issue can be reviewed before technical details are made public:

https://github.com/joeybomba

## Build transparency

This repository currently focuses on distributing official releases.

The full application source and complete reproducible Windows build pipeline are not yet published here. Planned transparency improvements include public build automation, release hashes, and build provenance or attestations where practical.
