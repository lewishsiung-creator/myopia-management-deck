# Myopia Management Market Overview — Taiwan

Interactive web deck built from Jolie Huang's PowerPoint, for her presentation to
management at CooperVision Taiwan.

**This repository is public**, at the owner's explicit instruction. Note that the deck
contains CooperVision internal material — FY26 revenue, channel-level market share,
BrightenOptix internal figures, and notes on the Zeiss / Brighten Optix acquisition.

## Hosting

`index.html` at the repo root is served two ways, both redeploying on every push to `main`:

- GitHub Pages — https://lewishsiung-creator.github.io/myopia-management-deck/
- Cloudflare Pages (project `jh-deck`) — https://jh-deck.pages.dev

`practice.html` is Jolie's rehearsal tool, at `/practice.html` on both hosts. It pairs
each slide with her spoken script at three levels (full text, key phrases, slide only)
and times her against a 115 wpm target. Deliberately a separate file from the deck —
her script must never be one keystroke away while she is presenting.

There is no access control and no noindex. The deck is open to anyone with the URL
and to search engines.

## Updating the deck

`index.html` is a single self-contained file: all 50 slides are embedded
as base64 JPEGs, exported from PowerPoint at 1920x1080. There are no other assets.
Replace that one file and push; Cloudflare redeploys in under a minute.

To regenerate it from a revised `.pptx`, the slides must be exported through
PowerPoint itself (LibreOffice drops the hidden slides and mangles the Morph
builds), then wrapped in the viewer shell.

## Presenting

Keyboard: arrows/space to advance, `A` all slides, `S` sections, `N` speaker notes,
`B` blackout, `F` full screen, `T` timer, `Backspace` to return from a jump, `?` for help.

Always carry the offline copy on a USB stick as well. The file works with no network.
