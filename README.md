# Gentle Shell Themes

Two planned community themes for Gentle Shell, inspired by SynthWave '84 and SynthWave '84 Blues for Visual Studio Code. The goal is to bring their distinctive palettes to the Pi terminal interface while keeping text readable for extended use.

## Project status

This project is in the planning stage. The themes have not yet been implemented, installed, or validated. Installation instructions and compatibility claims will be added after testing.

## Planned themes

- **SynthWave '84:** dark violet backgrounds with neon pink, cyan, green, and retro accents, adapted from the original theme by Robb Owen.
- **SynthWave '84 Blues:** a separate adaptation based on the actual Blues palette by sabrsorensen, not an assumed color shift of the original.

Both themes are intended to use native Pi theme JSON files with distinct names. Their colors will be mapped to interface roles, including messages, Markdown, syntax, tool output, and diffs. Visual adjustments made for contrast or usability will be documented.

## Scope and limitations

- Preserve the identity of each source theme while prioritizing legibility.
- Keep the themes independent of Gentle Shell and Pi source code.
- Do not implement the original editor's glow effect in the initial version. A standard Pi theme cannot reproduce it on its own.
- Do not assume that a Pi theme controls the background of the entire terminal window. Terminal color settings may need separate, optional configuration.
- Treat the project repository as the source of truth and local theme files as replaceable installed copies.

## Planned development

1. Inspect the installed Gentle Shell and Pi versions, the active agent home, and the matching theme schema.
2. Compare both original theme files and record their source versions and color mappings.
3. Build and validate the original theme first, then the Blues variant.
4. Test selection, persistence, contrast, messages, Markdown, tools, and diffs in Gentle Shell.
5. Document installation, recovery, compatibility, attribution, and any visual adjustments.
6. Investigate Pi package distribution after the themes have been validated.

Before changing an existing user configuration or replacing a local theme file, inspect and back up the affected files. Do not assume that a default Pi agent path applies to every Gentle Shell installation. A complete Gentle Shell uninstall may remove an isolated agent home, so installed files must not be the only copies.

## Credits and attribution

These planned themes are unofficial adaptations of:

- [SynthWave '84](https://github.com/robb0wen/synthwave-vscode), created by Robb Owen.
- [SynthWave '84 Blues](https://github.com/sabrsorensen/synthwave-blues-vscode-theme), adapted by sabrsorensen from SynthWave '84.

Both source repositories provide MIT license notices. The relevant notices will be preserved when source material is incorporated. This project is not affiliated with or endorsed by the original authors or the Gentle Shell project.

## License

New work in this repository is licensed under the [MIT License](LICENSE). The licenses of the original projects remain applicable to their respective material.
