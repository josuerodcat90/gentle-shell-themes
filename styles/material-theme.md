# Material Theme style guide

A dark palette for Gentle Shell adapted from the historical Material Theme Default variant. The [theme JSON](../themes/material-theme.json) is the source of truth.

## Interface and feedback

| Token | Value | Source |
| --- | --- | --- |
| `accent` | `#80CBC4` | `colors.accent` → `vars.teal` |
| `text` | `#EEFFFF` | `colors.text` → `vars.foreground` |
| `muted` | `#546E7A` | `colors.muted` → `vars.comment` |
| `border` | `#80CBC4` | `colors.border` → `vars.teal` |
| `borderAccent` | `#89DDFF` | `colors.borderAccent` → `vars.cyan` |
| `selectedBg` | `#374B50` | `colors.selectedBg` → `vars.selection` |
| `userMessageBg` | `#303C41` | `colors.userMessageBg` → `vars.userMessage` |
| `customMessageBg` | `#303F46` | `colors.customMessageBg` → `vars.customMessage` |
| `toolPendingBg` | `#303C41` | `colors.toolPendingBg` → `vars.toolPending` |
| `toolSuccessBg` | `#34463C` | `colors.toolSuccessBg` → `vars.toolSuccess` |
| `toolErrorBg` | `#49363A` | `colors.toolErrorBg` → `vars.toolError` |
| `success` | `#C3E88D` | `colors.success` → `vars.green` |
| `warning` | `#FFCB6B` | `colors.warning` → `vars.yellow` |
| `error` | `#F07178` | `colors.error` → `vars.red` |

## Markdown and syntax

| Token | Value | Source |
| --- | --- | --- |
| `mdHeading` | `#82AAFF` | `colors.mdHeading` → `vars.blue` |
| `mdLink` | `#80CBC4` | `colors.mdLink` → `vars.teal` |
| `mdCode` | `#C3E88D` | `colors.mdCode` → `vars.green` |
| `syntaxComment` | `#546E7A` | `colors.syntaxComment` → `vars.comment` |
| `syntaxKeyword` | `#89DDFF` | `colors.syntaxKeyword` → `vars.cyan` |
| `syntaxFunction` | `#82AAFF` | `colors.syntaxFunction` → `vars.blue` |
| `syntaxString` | `#C3E88D` | `colors.syntaxString` → `vars.green` |
| `syntaxNumber` | `#F78C6C` | `colors.syntaxNumber` → `vars.orange` |

These tables highlight common roles; the JSON contains all available mappings and palette variables.

## GPUI terminal ANSI overrides

These explicit variables are used by GPUI v0.1.24 for the indicated ANSI entries. Other entries may use existing palette variables or be derived by GPUI; ANSI 0 is not explicitly overridden. External terminals manage their own palettes.

| ANSI entry | Variable | Value |
| --- | --- | --- |
| 13 | `vars.brightMagenta` | `#D5ADEF` |

## Optional terminal colors

The recommended terminal background is `#263238` and foreground is `#EEFFFF`. These are optional terminal settings, not additional theme tokens. See [terminal appearance](../README.md#terminal-appearance).
