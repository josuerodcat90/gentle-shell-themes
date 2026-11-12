# Monokai style guide

A dark palette for Gentle Shell inspired by Monokai. The [theme JSON](../themes/monokai.json) is the source of truth; see the [preview](../images/monokai.png) for the theme in use.

## Interface and feedback

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `accent` | `#A6E22E` | Accent | `colors.accent` → `vars.green` |
| `text` | `#F8F8F2` | Main text | `colors.text` → `vars.foreground` |
| `muted` | `#88846F` | Muted text | `colors.muted` → `vars.comment` |
| `border` | `#768A4A` | Border | `colors.border` (literal) |
| `borderAccent` | `#A6E22E` | Accent borders | `colors.borderAccent` → `vars.green` |
| `selectedBg` | `#414339` | Selected background | `colors.selectedBg` → `vars.selection` |
| `userMessageBg` | `#383A30` | User message background | `colors.userMessageBg` → `vars.userMessage` |
| `customMessageBg` | `#39352F` | Custom message background | `colors.customMessageBg` → `vars.customMessage` |
| `toolPendingBg` | `#383A30` | Pending tool background | `colors.toolPendingBg` → `vars.toolPending` |
| `toolSuccessBg` | `#353D2B` | Successful tool background | `colors.toolSuccessBg` → `vars.toolSuccess` |
| `toolErrorBg` | `#472E32` | Failed tool background | `colors.toolErrorBg` → `vars.toolError` |
| `success` | `#A6E22E` | Success | `colors.success` → `vars.green` |
| `warning` | `#FD971F` | Warning | `colors.warning` → `vars.orange` |
| `error` | `#F92672` | Error | `colors.error` → `vars.red` |

## Markdown and syntax

| Token | Value | Usage | Source |
| --- | --- | --- | --- |
| `mdHeading` | `#F92672` | Markdown headings | `colors.mdHeading` → `vars.pink` |
| `mdLink` | `#66D9EF` | Markdown links | `colors.mdLink` → `vars.cyan` |
| `mdCode` | `#E6DB74` | Markdown code | `colors.mdCode` → `vars.yellow` |
| `syntaxComment` | `#88846F` | Syntax comments | `colors.syntaxComment` → `vars.comment` |
| `syntaxKeyword` | `#F92672` | Syntax keywords | `colors.syntaxKeyword` → `vars.pink` |
| `syntaxFunction` | `#A6E22E` | Syntax functions | `colors.syntaxFunction` → `vars.green` |
| `syntaxString` | `#E6DB74` | Syntax strings | `colors.syntaxString` → `vars.yellow` |
| `syntaxNumber` | `#AE81FF` | Syntax numbers | `colors.syntaxNumber` → `vars.purple` |

These tables highlight common roles; the JSON contains all available mappings and palette variables.

## Optional terminal colors

The recommended terminal background is `#272822` and foreground is `#F8F8F2`. These are terminal settings, not additional theme tokens. See [terminal appearance](../README.md#terminal-appearance).
