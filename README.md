# Gentle Shell Themes

An unofficial collection of Pi themes for Gentle Shell, inspired by SynthWave '84 and SynthWave '84 Blues for Visual Studio Code. The repository is the source of truth for theme files.

## Project status

- **SynthWave '84:** the first repository theme is [`themes/synthwave-84.json`](themes/synthwave-84.json). It has been checked against the installed Pi 1.5.0 schema, but its visual testing in Gentle Shell is still in progress.
- **SynthWave '84 Blues:** planned separately, based on the actual Blues palette by sabrsorensen, not an assumed color shift of the original.

The theme has been previewed on Windows; persistence and other platforms have not yet been verified. A Pi theme cannot reproduce the original editor glow on its own or necessarily control the entire terminal background.

## Install and use a theme

You need Git and an existing Gentle Shell installation. The instructions below install the available `synthwave-84` theme. The Blues theme is not available yet.

**Availability:** the theme has not yet been published to the default branch. A fresh clone will contain the theme only after the relevant changes have been published to the branch you check out.

### 1. Clone the repository

In PowerShell on Windows, or a terminal on Linux or macOS, run:

```sh
git clone https://github.com/josuerodcat90/gentle-shell-themes.git
cd gentle-shell-themes
```

If you already have a clone, open its directory instead. Check that `themes/synthwave-84.json` exists before continuing.

### 2. Find your agent home

Run this in the same environment you use to launch Gentle Shell:

```sh
gentle-shell home
```

The output includes a mode and a path, for example `isolated <agent-dir>`. Copy only the path, not the mode. The usual isolated home is `~/.gentle-shell/agent`, but linked or custom homes can differ. Use the reported path rather than assuming a location.

### 3. Copy the theme

Run the commands for your operating system from the cloned repository. Both options create the `themes` directory if needed and stop instead of replacing an existing theme with the same name. They do not edit `settings.json`.

#### Windows: PowerShell

```powershell
$agentHome = Read-Host 'Paste the agent home path from gentle-shell home'
$themesDir = Join-Path $agentHome 'themes'
$source = 'themes/synthwave-84.json'
$destination = Join-Path $themesDir 'synthwave-84.json'
if (!(Test-Path -LiteralPath $source -PathType Leaf)) { throw 'Theme file not found in this checkout.' }
if (!(Test-Path -LiteralPath $agentHome -PathType Container)) { throw 'Agent home directory not found.' }
New-Item -ItemType Directory -Force -Path $themesDir | Out-Null
if (Test-Path -LiteralPath $destination) { throw 'Theme already exists. Back it up before replacing it.' }
Copy-Item -LiteralPath $source -Destination $destination
```

#### Linux and macOS: shell

```sh
printf 'Paste the agent home path from gentle-shell home: '
IFS= read -r agent_home
if [ ! -f themes/synthwave-84.json ]; then
  echo 'Theme file not found in this checkout.'
elif [ ! -d "$agent_home" ]; then
  echo 'Agent home directory not found.'
elif [ -e "$agent_home/themes/synthwave-84.json" ]; then
  echo 'Theme already exists. Back it up before replacing it.'
else
  mkdir -p "$agent_home/themes" && cp -n themes/synthwave-84.json "$agent_home/themes/synthwave-84.json"
fi
```

If a theme with that name already exists, inspect and back it up before replacing it. The copy in this repository remains the source of truth.

### 4. Select the theme

Open Gentle Shell and choose `synthwave-84` through `/gentle:customize` or Pi's `/settings` theme selector. If a newly added theme is not listed, run `/reload` or restart Gentle Shell. To return to your previous theme, select it through the same interface.

### Update or recover

To update, obtain the desired repository version, back up any installed file with the same name, and copy the new JSON to the reported agent home's `themes` directory. After a reinstall or home change, run `gentle-shell home` again before copying. A complete Gentle Shell uninstall may remove an isolated agent home, so keep your repository copy separately. Avoid installing the same theme through multiple sources at once, as duplicate names can conflict.

## Next steps

1. Continue testing persistence, contrast, messages, Markdown, tools and diffs in Gentle Shell.
2. Verify installation on Linux and macOS and document compatibility.
3. Build and validate the separate Blues theme, then investigate Pi package distribution.

## Credits and attribution

These themes are unofficial adaptations of:

- [SynthWave '84](https://github.com/robb0wen/synthwave-vscode), created by Robb Owen. Its [MIT notice](LICENSES/synthwave-84-MIT.txt) is preserved here.
- [SynthWave '84 Blues](https://github.com/sabrsorensen/synthwave-blues-vscode-theme), adapted by sabrsorensen from SynthWave '84. This variant is planned and its notice will be preserved when its source material is incorporated.

This project is not affiliated with or endorsed by the original authors or the Gentle Shell project.

## License

New work in this repository is licensed under the [MIT License](LICENSE). The licenses of the original projects remain applicable to their respective material.
