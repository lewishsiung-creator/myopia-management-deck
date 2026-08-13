# Myopia Management Market Overview — Taiwan

Interactive web deck built from Jolie Huang's PowerPoint, for her presentation to
management at CooperVision Taiwan.

**This repository is private and must stay private.** The deck contains CooperVision
internal material — FY26 revenue, channel-level market share, BrightenOptix internal
data, and commercially sensitive notes on the Zeiss / Brighten Optix acquisition.

## Hosting

`public/` is deployed to Cloudflare Pages on every push to `main`.
The site sits behind Cloudflare Access — viewers must confirm an allowlisted
email address before anything loads. `robots.txt` and `_headers` add
noindex on top of that, as a second line of defence rather than a first.

## Updating the deck

`public/index.html` is a single self-contained file: all 50 slides are embedded
as base64 JPEGs, exported from PowerPoint at 1920x1080. There are no other assets.
Replace that one file and push; Cloudflare redeploys in under a minute.

To regenerate it from a revised `.pptx`, the slides must be exported through
PowerPoint itself (LibreOffice drops the hidden slides and mangles the Morph
builds), then wrapped in the viewer shell.

## Presenting

Keyboard: arrows/space to advance, `A` all slides, `S` sections, `N` speaker notes,
`B` blackout, `F` full screen, `T` timer, `Backspace` to return from a jump, `?` for help.

Always carry the offline copy on a USB stick as well. The file works with no network.
