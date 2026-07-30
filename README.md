
# release-dl

An interactive cross-platform github release downloader made in pwsh for convenience
![Demo usage of release-dl](rel-demo.gif)

## Usage
In powershell or pwsh
```
rel
```
It prompts for repository search title

#### Keys
`Enter` to select repository/release/asset \
`Up/Down` to naviagate results of repository/release/asset \
`O` to open repository in default browser \
`Tab` to multi-select asset/source/release-description-asset for bulk download \
`Escape` to cancel operation and exit


## Installation

#### Linux:

Arch/linux:
```bash
yay -S powershell-bin
```

Ubuntu/debian:
```bash
sudo apt-get install -y powershell
```
Then run:
```bash
  mkdir -p "$HOME/.local/bin" && curl -fsSL "https://raw.githubusercontent.com/devvratmiglani/release-dl/refs/heads/main/src/rel" -o "$HOME/.local/bin/rel" && chmod +x "$HOME/.local/bin/rel"
```

#### Windows:
In powershell:

```bash
$bin = "$env:LOCALAPPDATA\Microsoft\WindowsApps"
Invoke-WebRequest "https://raw.githubusercontent.com/devvratmiglani/release-dl/refs/heads/main/src/rel" -OutFile "$bin\rel.ps1"
```
If `$env:LOCALAPPDATA\Microsoft\WindowsApps` is not in environment paths, replace `$bin` with a directory in paths or add it to paths.

