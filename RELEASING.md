# Release Process

This repository publishes Data Explorer binaries that are built from the private source repository.

## Version 1.8.0

Local release asset:

```text
Data Explorer (1.8.0).exe
```

SHA-256:

```text
fa5a9fe1e2ff799a78253b46eed8084e25296d3ff0759a5e6c3df523c2a91039
```

## Maintainer Checklist

1. Build the Windows executable from the private source repository.
2. Copy the executable into this repository using the naming pattern `Data Explorer (<version>).exe`.
3. Compute the checksum:

   ```bash
   sha256sum "Data Explorer (<version>).exe"
   ```

4. Update `README.md`, `CHANGELOG.md`, and `.github/release-notes/v<version>.md`.
5. Commit the documentation changes.
6. Create an annotated tag:

   ```bash
   git tag -a v<version> -m "Data Explorer v<version>"
   ```

7. Push `main` and the tag:

   ```bash
   git push origin main v<version>
   ```

8. Upload the executable as a GitHub Release asset.

With GitHub CLI:

```bash
gh release create v<version> "Data Explorer (<version>).exe" \
  --title "Data Explorer <version>" \
  --notes-file ".github/release-notes/v<version>.md" \
  --latest
```

Without GitHub CLI, create the release from the GitHub web UI and upload the executable in the release assets area.
