# Data Explorer Releases

Public release repository for **Data Explorer**, a Windows desktop application distributed as a pre-built executable.

The Python source code is maintained in a separate private repository. This repository is only for public release metadata, changelogs, license information, and GitHub Release assets.

## Download

- Latest release: <https://github.com/anthony-bouh/cetim-data-explorer-releases/releases/latest>
- Version 1.8.0 executable: <https://github.com/anthony-bouh/cetim-data-explorer-releases/releases/download/v1.8.0/Data%20Explorer%20(1.8.0).exe>

## Installation

1. Download `Data Explorer (1.8.0).exe` from the GitHub release assets.
2. Run the executable on Windows.
3. If Windows SmartScreen appears, verify the checksum below before choosing to run the application.

## Checksum

SHA-256 for `Data Explorer (1.8.0).exe`:

```text
fa5a9fe1e2ff799a78253b46eed8084e25296d3ff0759a5e6c3df523c2a91039
```

On Windows PowerShell:

```powershell
Get-FileHash ".\Data Explorer (1.8.0).exe" -Algorithm SHA256
```

## Repository Scope

This repository intentionally does not contain:

- Python source files
- Build scripts from the private application repository
- Large binary artifacts committed to Git history

Release binaries are uploaded as GitHub Release assets instead of being committed to the repository.

## License

See [LICENSE](LICENSE).
