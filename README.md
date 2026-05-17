# Recipe Rage Cleaner

> Extract just the recipe. Skip the 3,000-word life story.

**Day 04 / 180 — 180 Days of Building**

Every food blog buries the recipe under a novel about their grandmother's kitchen, a trip to Tuscany, and three paragraphs about seasonal produce. This extension cuts straight to ingredients and steps — and rates your rage level for what you just had to sit through.

![Demo](demo.gif)

---

## What it does

- **Rage Meter** — scores how much unnecessary content came before the recipe (0–10)
- **Ingredients** — clean bullet list with exact measurements, nothing extra
- **Instructions** — numbered steps only, no filler
- **What You Skipped** — sarcastic summary of the fluff you just escaped
- **Wrong kitchen detector** — open a non-food page? It humorously lists the "ingredients" of whatever you're looking at instead

---

## How to use

1. Open any food blog or recipe page
2. Click the extension icon
3. Hit **Extract Recipe**
4. Get the recipe instantly — no scrolling, no waiting for ads to load

---

## Setup

### 1. Load the extension
1. Go to `chrome://extensions`
2. Enable **Developer mode** (top right toggle)
3. Click **Load unpacked** → select the `recipe-rage-cleaner` folder

### 2. Add your API key
Click **⚙** in the popup and paste one of the following:

- **Gemini API key** — free at [aistudio.google.com](https://aistudio.google.com/apikey)
- **OpenRouter API key** — free tier at [openrouter.ai](https://openrouter.ai) (use as fallback if Gemini quota runs out)

Only one key is required. If both are saved, Gemini is used first with OpenRouter as fallback.

---

## Tech stack

- Chrome Extension Manifest V3
- Gemini 2.0 Flash (primary) → OpenRouter fallback
- Two-phase progressive loading: instant word count preview → full recipe extraction
- Vanilla JS — no frameworks, no build step

---

## Part of 180 Days of Building

Shipping one AI Chrome extension every day for 180 days.

Follow along: [@happy_ships](https://x.com/happy_ships)
