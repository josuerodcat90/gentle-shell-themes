# Dracula style guide

A dark palette for Gentle Shell inspired by Dracula. The [theme JSON](../themes/dracula.json) is the source of truth; see the [preview](../images/dracula.png) for the theme in use.

## Interface and feedback

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `accent` | `#bd93f9` | Accent | `colors.accent` → `vars.purple` |
| `text` | `#f8f8f2` | Main text | `colors.text` → `vars.foreground` |
| `muted` | `#6272a4` | Muted text | `colors.muted` → `vars.comment` |
| `borderAccent` | `#bd93f9` | Accent borders | `colors.borderAccent` → `vars.purple` |
| `selectedBg` | `#44475a` | Selected background | `colors.selectedBg` → `vars.selection` |
| `userMessageBg` | `#383a4d` | User message background | `colors.userMessageBg` → `vars.userMessage` |
| `customMessageBg` | `#3a384c` | Custom message background | `colors.customMessageBg` → `vars.customMessage` |
| `toolPendingBg` | `#383a4d` | Pending tool background | `colors.toolPendingBg` → `vars.toolPending` |
| `toolSuccessBg` | `#30413c` | Successful tool background | `colors.toolSuccessBg` → `vars.toolSuccess` |
| `toolErrorBg` | `#49343e` | Failed tool background | `colors.toolErrorBg` → `vars.toolError` |
| `success` | `#50fa7b` | Success | `colors.success` → `vars.green` |
| `warning` | `#ffb86c` | Warning | `colors.warning` → `vars.orange` |
| `error` | `#ff5555` | Error | `colors.error` → `vars.red` |

## Markdown and syntax

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `mdHeading` | `#ff79c6` | Markdown headings | `colors.mdHeading` → `vars.pink` |
| `mdLink` | `#8be9fd` | Markdown links | `colors.mdLink` → `vars.cyan` |
| `mdCode` | `#f1fa8c` | Markdown code | `colors.mdCode` → `vars.yellow` |
| `syntaxComment` | `#6272a4` | Syntax comments | `colors.syntaxComment` → `vars.comment` |
| `syntaxKeyword` | `#ff79c6` | Syntax keywords | `colors.syntaxKeyword` → `vars.pink` |
| `syntaxFunction` | `#50fa7b` | Syntax functions | `colors.syntaxFunction` → `vars.green` |
| `syntaxString` | `#f1fa8c` | Syntax strings | `colors.syntaxString` → `vars.yellow` |
| `syntaxNumber` | `#bd93f9` | Syntax numbers | `colors.syntaxNumber` → `vars.purple` |

These tables highlight common roles; the JSON contains all available mappings and palette variables.

## Optional terminal colors

The recommended terminal background is `#282A36` and foreground is `#F8F8F2`. These are terminal settings, not additional theme tokens. See [terminal appearance](../README.md#terminal-appearance).
