# CCC Releases

Public release binaries for the [CCC](https://getc3.app) suite.

This repository hosts downloads for two products; their releases are namespaced
by tag so they never collide:

| Product | What it is | Release tags |
|---|---|---|
| **CCC** | Control your AI coding agents from your mobile device | `v*` |
| **C3Sync** | Cross-machine, end-to-end-encrypted sync of AI coding-agent sessions and files | `c3sync-v*` |

---

## CCC — Code Chat Connect

Control your AI coding agents — Claude Code, Codex, OpenCode, and Pi — from
your mobile device: monitor sessions, respond to prompts, and manage your
development workflow on the go.

### Quick install

**macOS / Linux / WSL:**
```bash
curl -fsSL https://getc3.app/install.sh | bash
```

**Windows (PowerShell):**
```powershell
irm https://getc3.app/install.ps1 | iex
```

### Manual download

Grab the binary for your platform from the
[releases page](https://github.com/ccc-app/ccc-releases/releases) (tag `v*`):

| Platform | Binary |
|---|---|
| Linux x64 | `ccc-linux-x64` |
| Linux ARM64 | `ccc-linux-arm64` |
| macOS Intel | `ccc-darwin-x64` |
| macOS Apple Silicon | `ccc-darwin-arm64` |
| Windows x64 | `ccc-windows-x64.exe` |

Learn more at [getc3.app](https://getc3.app).

---

## C3Sync

Pick up any AI coding-agent session — and the exact file state that went with
it — on any machine you own. Agent-agnostic (Claude Code, Codex, OpenCode, Pi),
end-to-end encrypted, works offline.

### Quick install

Installs both binaries (`c3sync` CLI and `c3syncd` daemon) and verifies the
download against published sha256 checksums.

**macOS / Linux / WSL:**
```bash
curl -fsSL https://getc3.app/sync/install.sh | bash
```

**Windows (PowerShell):**
```powershell
irm https://getc3.app/sync/install.ps1 | iex
```

There is no stable release yet — add `--beta` (bash) or set
`$env:C3SYNC_CHANNEL='beta'` (PowerShell) to install the latest beta.

### Manual download

Each archive (tag `c3sync-v*`) contains both binaries plus a
`c3sync_<version>_checksums.txt` for verification:

| Platform | Archive |
|---|---|
| Linux x64 | `c3sync_<version>_linux_amd64.tar.gz` |
| Linux ARM64 | `c3sync_<version>_linux_arm64.tar.gz` |
| macOS Intel | `c3sync_<version>_darwin_amd64.tar.gz` |
| macOS Apple Silicon | `c3sync_<version>_darwin_arm64.tar.gz` |
| Windows x64 | `c3sync_<version>_windows_amd64.zip` |
| Windows ARM64 | `c3sync_<version>_windows_arm64.zip` |

Linux is the supported beta platform. Source and full documentation:
[github.com/ccc-app/c3sync](https://github.com/ccc-app/c3sync).
