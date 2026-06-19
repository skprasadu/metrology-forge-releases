# P2I Engineering Tools

Public release repository for small, local-first engineering utilities.

This repository hosts downloadable builds, checksums, and release notes. It does not contain the source code.

## Metrology Forge

Metrology Forge is the first P2I tool. It parses PC-DMIS-style CMM report exports and produces redacted diagnostics that are safe to share for parser feedback.

Current focus:

- PC-DMIS-style report parsing

- Redacted diagnostic generation

- Source-line evidence for parser issues

- Windows desktop installer

- Windows CLI package

## Downloads

Use the Releases page:

[View releases](https://github.com/skprasadu/metrology-forge-releases/releases)

Each release normally includes:

| Asset | Purpose |

| --- | --- |

| `MetrologyForge-windows-x64.msi` | Windows desktop installer |

| `met-cli-windows-x64.zip` | Command-line parser/redaction tool |

| `SHA256SUMS.txt` | Checksums for release files |

| `RELEASE_NOTES.md` | Release-specific notes |

## CLI example

```powershell

met.exe inspect-redacted report.txt --out redacted-diagnostic.json
