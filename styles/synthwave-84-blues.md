# SynthWave '84 Blues style guide

A dark blue, neon palette for Gentle Shell. The [theme JSON](../themes/synthwave-84-blues.json) is the source of truth; see the [preview](../images/synthwave-84-blues.png) for the theme in use.

## Interface and feedback

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `accent` | `#36f9f6` | Accent | `colors.accent` → `vars.aqua` |
| `text` | `#ffffff` | Main text | `colors.text` → `vars.white` |
| `muted` | `#848bbd` | Muted text | `colors.muted` → `vars.comment` |
| `borderAccent` | `#7ed0ff` | Accent borders | `colors.borderAccent` → `vars.blue` |
| `selectedBg` | `#003564` | Selected background | `colors.selectedBg` → `vars.selection` |
| `userMessageBg` | `#002b4e` | User message background | `colors.userMessageBg` → `vars.userMessage` |
| `customMessageBg` | `#26334a` | Custom message background | `colors.customMessageBg` → `vars.customMessage` |
| `toolPendingBg` | `#173649` | Pending tool background | `colors.toolPendingBg` → `vars.toolPending` |
| `toolSuccessBg` | `#193c3c` | Successful tool background | `colors.toolSuccessBg` → `vars.toolSuccess` |
| `toolErrorBg` | `#432d3a` | Failed tool background | `colors.toolErrorBg` → `vars.toolError` |
| `success` | `#72f1b8` | Success | `colors.success` → `vars.green` |
| `warning` | `#fede5d` | Warning | `colors.warning` → `vars.yellow` |
| `error` | `#fe4450` | Error | `colors.error` → `vars.red` |

## Markdown and syntax

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `mdHeading` | `#7ed0ff` | Markdown headings | `colors.mdHeading` → `vars.blue` |
| `mdLink` | `#fede5d` | Markdown links | `colors.mdLink` → `vars.yellow` |
| `mdCode` | `#ff8b39` | Markdown code | `colors.mdCode` → `vars.orange` |
| `syntaxComment` | `#848bbd` | Syntax comments | `colors.syntaxComment` → `vars.comment` |
| `syntaxKeyword` | `#fede5d` | Syntax keywords | `colors.syntaxKeyword` → `vars.yellow` |
| `syntaxFunction` | `#36f9f6` | Syntax functions | `colors.syntaxFunction` → `vars.aqua` |
| `syntaxString` | `#ff8b39` | Syntax strings | `colors.syntaxString` → `vars.orange` |
| `syntaxNumber` | `#f97e72` | Syntax numbers | `colors.syntaxNumber` → `vars.coral` |
| `syntaxType` | `#d64a53` | Syntax types | `colors.syntaxType` → `vars.typeRed` |

These tables highlight common roles; the JSON contains all available mappings and palette variables.

## Optional terminal colors

The recommended terminal background is `#002335` and foreground is `#E5E5E5`. These are terminal settings, not additional theme tokens. See [terminal appearance](../README.md#terminal-appearance).
