# tamp

***Small tools for people who think in plain text.***

---

tamp is a collection of command-line tools built around one idea: your notes, tasks, and thoughts should live in plain markdown files that you own, on your machine, forever. No account. No sync service. No lock-in.

---

### tools

| | status | description |
|---|---|---|
| [**tamp-note**](https://github.com/tamp-workshop/tamp) | active | Daily notes TUI. Quick-add from anywhere, slash commands, tag autocomplete, local stats. |

All tools share the same file format and data layer. Your notes work with all of them — and with none of them.

---

### themes

Three cinematic colour families for VSCode and Vim.

[**tamp-workshop/themes**](https://github.com/tamp-workshop/themes) — Lunar Lobby · Space Rumours · Vanguard Outpost

---

### why we changed course

tamp started as a single shell script called `note`. It worked, people used it, and it grew. But a single script can't cleanly become multiple tools sharing the same data.

In March 2026 I rewrote everything as a proper monorepo:
- **tamp-core** *shared data layer, one implementation of the file format*
- **tamp-note** *the TUI tool, rebuilt from scratch on Textual*
- Future tools will import from tamp-core without duplicating any logic. Hopefully...

The old `note` repo is archived. Everything is in [tamp-workshop/tamp](https://github.com/tamp-workshop/tamp) now.

---

*Good contributions welcome. No new dependencies without a strong reason. If you're not sure whether something belongs in tamp, it probably doesn't.*
