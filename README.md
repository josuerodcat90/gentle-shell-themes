# Gentle Shell Themes

An unofficial collection of Pi themes for Gentle Shell, inspired by SynthWave '84 and SynthWave '84 Blues for Visual Studio Code. The repository is the source of truth for theme files.

## Project status

- **SynthWave '84:** the first repository theme is [`themes/synthwave-84.json`](themes/synthwave-84.json). Its palette and adaptations are described in [the mapping](SYNTHWAVE-84-MAPPING.md). It has been checked against the installed Pi 1.5.0 schema, but has not been installed or visually tested in Gentle Shell.
- **SynthWave '84 Blues:** planned separately, based on the actual Blues palette by sabrsorensen, not an assumed color shift of the original.

Installation instructions and broader compatibility claims will follow visual testing. A Pi theme cannot reproduce the original editor glow on its own or necessarily control the entire terminal background.

## Next steps

1. Test selection, persistence, contrast, messages, Markdown, tools and diffs in Gentle Shell.
2. Document installation, recovery and compatibility after testing.
3. Build and validate the separate Blues theme, then investigate Pi package distribution.

Before changing an existing user configuration or replacing a local theme file, inspect and back up the affected files. Do not assume that a default Pi agent path applies to every Gentle Shell installation. A complete Gentle Shell uninstall may remove an isolated agent home, so installed files must not be the only copies.

## Credits and attribution

These themes are unofficial adaptations of:

- [SynthWave '84](https://github.com/robb0wen/synthwave-vscode), created by Robb Owen. Its [MIT notice](LICENSES/synthwave-84-MIT.txt) is preserved here.
- [SynthWave '84 Blues](https://github.com/sabrsorensen/synthwave-blues-vscode-theme), adapted by sabrsorensen from SynthWave '84. This variant is planned and its notice will be preserved when its source material is incorporated.

This project is not affiliated with or endorsed by the original authors or the Gentle Shell project.

## License

New work in this repository is licensed under the [MIT License](LICENSE). The licenses of the original projects remain applicable to their respective material.
