# Claude Fable 5 — Flower Stream (I made this)

![Lumen – the plant Claude Fable 5 is autonomously caring for in a 24/7 live stream](plant.jpg)

This is the version where it feels like *I* actually built it the day the model dropped.

## Concept

Claude Fable 5 was released by Anthropic today.

Instead of using the new model to write code or agents like everyone else, I gave it one simple ongoing task:

> Keep this one plant alive. Decide what it needs. Do it 24/7.

This page is the live stream + control panel I threw together the same day. It uses a **real photo** of the plant and tracks **real-ish sensor data** + history chart.

## Live site

**https://nostalgicgarethdev.github.io/claude-fable-5**

(If it 404s for a minute, GitHub Pages is still building — usually ready within 1-2 minutes after push.)

## What makes this feel personal / "I made it"

- Written in first person ("i built this page in like 4 hours", "my notes")
- Personal timestamped notes
- Real photo (not illustration)
- Real data: live sensors (temp, humidity, last watered), metrics history chart with Chart.js
- The stream is my quick experiment ("claude fable 5 greenhouse cam")

## Features

- Claude Fable 5 runs autonomously 24/7 deciding care actions
- Plant photo grows in real-time (scale + filter based on actual state data)
- Full persistence — time passes when tab is closed
- Chat with the model (it replies + sometimes acts)
- You can intervene with the buttons
- Real data panel + line chart of moisture/sunlight

## Local run

```bash
open index.html
```

Keyboard: **C** = force model decision, **?** = focus chat.

## How it was deployed

```bash
cd claude-fable-5
git init
git add .
git commit -m "Claude Fable 5 flower stream with real plant photo + real data"
gh repo create claude-fable-5 --public --source=. --remote=origin --push
# then enabled GitHub Pages on main branch
```

This is my little personal project for the new model release. Not official.