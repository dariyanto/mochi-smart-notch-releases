# Security policy

## Reporting a vulnerability

Please report security problems privately, not in a public issue. Use
[GitHub private vulnerability reporting](https://github.com/dariyanto/mochi-smart-notch-releases/security/advisories/new)
on this repository. You will get a reply within a few days.

## Verifying a download

Each release lists the SHA-256 of the installer in its notes. In PowerShell:

```powershell
Get-FileHash .\Mochi-Smart-Notch_<version>_x64-setup.exe -Algorithm SHA256
```

The hash must match the one in the release notes. In-app updates are checked against a signature
before they are installed.
