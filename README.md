<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/logo-dark.png">
    <img src="assets/logo-light.png" width="220" alt="Ponytail Lite">
  </picture>
</p>

<h1 align="center">Ponytail Lite</h1>

<p align="center">
  <em>One file. No hooks. He would have wanted it this way.</em>
</p>

<br>

"Ponytail Lite" is [Ponytail](https://github.com/DietrichGebert/ponytail) without the plugin madness.

Not to be confused with Ponytail's `lite` mode. This is a separate one-file version:

No plugin. No hooks. No MCP. No commands. No mode switching. Just copy [`AGENTS.md`](AGENTS.md) into the place your agent reads instructions. That's it.

## The Joke

Ponytail is a beautiful contradiction: an anti-overengineering tool delivered as a whole plugin ecosystem, with lifecycle hooks, slash commands, MCP, statuslines, adapter tests, and enough install paths to make a senior engineer stare silently at the wall.

Ponytail Lite is what happens after that senior engineer comes back from coffee:

```text
AGENTS.md
```

## Why This Exists

Could you just copy `AGENTS.md` from [Ponytail](https://github.com/DietrichGebert/ponytail)? Yes.

This repo exists so you do not have to walk past the plugin machinery to find the one file.

The `AGENTS.md` here is not a byte-for-byte copy. It is an opinionated cleanup of the original: same lazy senior dev idea, less plugin baggage, and guardrails rewritten for people who just want the file.

## Install

Copy [`AGENTS.md`](AGENTS.md), or copy the same text into whatever your agent calls "project instructions" or "rules".

| Agent              | Put the Ponytail Lite text here                                                         |
| ------------------ | --------------------------------------------------------------------------------------- |
| Aider              | Your project instructions / conventions file                                            |
| Antigravity CLI    | `AGENTS.md` or `.agents/rules/ponytail.md`                                              |
| Claude Code        | `CLAUDE.md` or project instructions                                                     |
| Cline              | `.clinerules/ponytail.md`                                                               |
| CodeWhale          | `AGENTS.md`                                                                             |
| Codex              | `AGENTS.md` or Settings > Personalization > Custom instructions                         |
| Cursor             | `.cursor/rules/ponytail.mdc`                                                            |
| Devin CLI          | Custom instructions / project instructions                                              |
| Gemini CLI         | `AGENTS.md`                                                                             |
| GitHub Copilot     | `.github/copilot-instructions.md`                                                       |
| GitHub Copilot CLI | `AGENTS.md`, `.github/copilot-instructions.md`, or `~/.copilot/copilot-instructions.md` |
| Hermes Agent       | Custom instructions / system prompt                                                     |
| Kiro               | `.kiro/steering/ponytail.md`                                                            |
| OpenClaw           | Custom skill / instruction file                                                         |
| OpenCode           | `AGENTS.md` or OpenCode instructions                                                    |
| Pi agent           | Custom instructions / system prompt                                                     |
| Swival             | `AGENTS.md` or `~/.config/swival/AGENTS.md`                                             |
| Windsurf           | `.windsurf/rules/ponytail.md`                                                           |
| Zed                | Custom instructions / rules                                                             |

## Uninstall

Delete the file you copied.

If you pasted the text into a global instructions file, delete that paragraph.

No cleanup script. No leftover mode flag. No statusline entry. No hidden MCP server still thinking about your dependency graph.

## What It Does

Before writing code, the agent climbs this ladder:

1. Does this need to exist?
2. Does it already exist in the codebase?
3. Does the standard library do it?
4. Does a native platform feature cover it?
5. Does an installed dependency solve it?
6. Can this be one line?
7. Only then, write the minimum code that works.

## License

MIT
