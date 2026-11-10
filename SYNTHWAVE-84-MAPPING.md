# SynthWave '84 mapping

`themes/synthwave-84.json` adapts the [original VS Code theme](https://github.com/robb0wen/synthwave-vscode/blob/ecfa2fe1279f7233663fa3f98a96e6756000567b/themes/synthwave-color-theme.json) at commit `ecfa2fe1279f7233663fa3f98a96e6756000567b`. The [upstream MIT notice](LICENSES/synthwave-84-MIT.txt) applies to its source material.

## Palette and semantic mapping

Every color is an opaque RGB value present in the pinned source. Pi roles group many VS Code scopes, so the mapping is an adaptation rather than a one-to-one conversion.

| Variable | RGB | Source and Pi usage |
| --- | --- | --- |
| editor | `#262335` | Editor background; custom messages and successful tool boxes |
| panel | `#2a2139` | Input background; user messages and pending/error tool boxes |
| selection | `#463564` | Editor hover highlight; selected item background |
| border | `#495495` | Editor group border; borders, horizontal rules and a thinking level |
| white | `#ffffff` | Foreground; primary text and tool output |
| pink | `#ff7edb` | Variables and headings; accents, labels, list bullets and high thinking |
| cyan | `#03edf9` | Terminal cyan; custom labels and a thinking level |
| aqua | `#36f9f6` | Functions; syntax functions |
| green | `#72f1b8` | Terminal green and Markdown quotes; success, added diffs, links and quotes |
| yellow | `#fede5d` | Keywords and Markdown link titles; warnings, keywords, operators and link labels |
| red | `#fe4450` | Errors and types; errors, removed diffs and syntax types |
| comment | `#848bbd` | Comments; secondary text, borders and thinking text |
| orange | `#ff8b39` | Strings; syntax strings and inline code |
| coral | `#f97e72` | Numbers and cursor; syntax numbers and bash mode |
| gray | `#b6b1b1` | Template and key-value punctuation; punctuation, dim text and diff context |

## Deviations and limits

- Translucent VS Code selection, diff, and other overlays cannot be used as opaque Pi RGB colors unchanged. Selection uses the source's opaque hover color; diffs use its green and red foregrounds instead of alpha backgrounds. Tool states use existing dark backgrounds, not translucent state overlays.
- Pi has fewer syntax and Markdown roles than VS Code; language-specific overrides, font styles and the original glow are not reproduced. Markdown inline code uses the string color, and generic types use the source class color.
- Thinking levels, message boxes, borders and bash mode have no direct VS Code equivalents. Their colors are assigned from the source palette. Optional Pi colors use schema fallbacks.
- A Pi theme does not set the entire terminal background. Contrast, selection behavior and rendering still need visual testing in Gentle Shell; schema validation does not establish usability.
