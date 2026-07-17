# LWS Profile Studio

Upload a photo, get an alliance-branded profile avatar. Zero server-side processing — everything runs in the browser.

**Live:** https://bullochman.github.io/lws-profile-studio-static/

## Features

- **Upload any photo** (JPG / PNG / HEIC up to 20 MB)
- **Auto-crop to circle** with zoom + pan controls
- **Duotone treatment** in three alliance-brand palettes (Gold, Ice, Crimson)
- **Season 2 frost overlay** for the wintery LWS theme
- **Rank badge** (R5 / R4 / R3 / R2 / R1) in the bottom-right corner
- **Alliance name text** arcing along the top of the ring
- **Player name** flat along the bottom
- **Download PNG** (512×512, Discord-ready)
- **Post to Discord** — via the shared `lws-discord.js` webhook integration
- **Bilingual EN + KR** from day one

## Privacy

Every operation runs on the visitor's device. **The photo never leaves the browser** — no upload endpoint, no CDN, no telemetry on the image. The only outbound HTTPS request is the optional Discord webhook post, and that only happens when the user clicks "Post to Discord" after configuring their own webhook URL.

## Why it's the viral tool

Every alliance member visits to make their own avatar → posts to Discord → 30 members see it → they visit r5tools.io → make theirs. The alliance-wide uniform look is the visual signature that says "this alliance is organized."

## Local development

```
cd LWS_Profile_Studio
python3 -m http.server 8090
# open http://localhost:8090/
```

Static site, no build step, no dependencies beyond the browser.

## Related tools

- [Roster Extractor](https://roster.r5tools.io/) — video → CSV, feeds every LWS tool
- [Hive Grid Manager](https://hive.r5tools.io/) — formations by rank tier
- [Landing Planner](https://bullochman.github.io/lws-landing-planner-static/) — S2 Day-1 assignments

Part of the [R5TOOLS.IO](https://r5tools.io) Last War: Survival alliance toolkit.
