# ScriptBot — Performance Marketing Script Generator

AI-powered ad script generator for Performance, Remarketing, and App Install campaigns. Built on Claude AI with a full learning loop.

## Features
- **Script Generator** — AI writes structured 15–90s scripts (Hook → Agitate → Solution → Proof → CTA)
- **Hook Builder** — 4 proven formulas + AI hook generator + swipe file
- **Script Blueprint** — Step-by-step frameworks for each campaign type
- **Learning Loop** — Feeds campaign performance data back into generation
- **Script Library** — Persistent storage with ratings and Gold tagging
- **Insights** — Performance charts + extracted learned rules

## Setup

1. Deploy to Netlify (drag & drop the folder or connect GitHub)
2. Open the app → go to **Settings**
3. Enter your [Anthropic API key](https://console.anthropic.com) (starts with `sk-ant-`)
4. Start generating scripts

## How the Learning Loop Works

1. Generate a script → rate it → save to Library
2. Run the campaign, collect metrics (CTR, CVR, ROAS)
3. Go to Insights → enter Script ID + performance data
4. ScriptBot extracts a learned rule and injects it into all future generations
5. Scripts improve with every campaign cycle

## Data Storage

All data is stored in browser `localStorage` — nothing is sent to any server except directly to Anthropic's API for generation. Export your library anytime from Settings.

## Tech Stack

- Vanilla HTML/CSS/JS (no framework, no build step)
- Anthropic Claude API (claude-sonnet-4 by default)
- Browser localStorage for persistence
