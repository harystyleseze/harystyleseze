# GitHub profile README: decisions and checklist

## What I changed from the ChatGPT brief
1. **It had no idea, only rules.** The brief listed what to avoid but never said what the page is. Here the page is a *revised manuscript*: the brand's insertion lockup at the top, three verbs as the whole structure (I build · I contribute · I write), a signature at the end, and a "Last revised" date. Revising until it's right is the brand idea, so the page shows it.
2. **It missed your strongest repo.** CareGuard (745 commits, CI, tests, ADRs, OpenAPI, live demo) isn't in your master document. It now leads Selected work.
3. **Its A–G section list was a conventional README in nicer words.** I collapsed it to four sections plus contact. The structure comes from your own brand positioning: build, contribute, communicate.
4. **"Use the colours as a starting point" was too vague for GitHub.** A README can't set backgrounds, so the header uses transparent SVGs. A `<picture>` with `prefers-color-scheme` swaps ink for paper in dark mode, so the type sits *on* GitHub's page instead of inside a banner box.
5. **Fonts.** GitHub won't load webfonts inside SVGs. The headers embed tiny subset fonts (about 4 KB each), so the SVGs are fully self-contained.
6. **Honesty is part of the format.** Limitations sit in native blockquotes under the project they apply to. The "I write" section admits nothing is published yet instead of faking links.
7. **Skills are a 4-line working set, not a badge wall.** It includes only tools seen in your repos or roles. Go and C are dropped because they're training-only.

## Files to put in the `harystyleseze/harystyleseze` repo
```
README.md
assets/header-light.svg
assets/header-dark.svg
assets/signature-light.svg
assets/signature-dark.svg
```
`Preview.html` and `NOTES.md` are for review only. Don't commit them.

## Needs your input
- **Dispatch:** a repository link. I couldn't find one.
- **CareGuard:** confirm your role. I wrote "built in the open". If others co-built it, say so.
- **NodeBridge:** confirm the validator wording ("operated").
- **ChainGuard:** a repo link, if public.
- **Writing:** the first published piece, to replace the placeholder line.
- **Contact:** a professional email, if you want one listed.

## Before you publish
- [ ] Header and signature render in light **and** dark (GitHub → Settings → Appearance).
- [ ] View on mobile: the header scales to width, and the text below repeats everything in it.
- [ ] Every link opens. Live demos: careguard-seven.vercel.app, dcfr.onrender.com. Render may cold-start.
- [ ] With images off, the alt text still says who you are.
- [ ] Update the "Last revised" line whenever you change the page.
