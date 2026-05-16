# Recipe Rage Cleaner

> Extract just the recipe. Skip the 3,000-word life story.

A Chrome extension that strips food blog nonsense and gives you only what you came for — ingredients and steps. Also rates your rage level (out of 10) and lists the worst filler you just skipped.

![Demo](demo.gif)

## What it does

- **🔥 Rage Meter** — scores how much unnecessary content came before the recipe (0–10)
- **Ingredients** — clean bullet list with exact measurements
- **Instructions** — numbered steps, nothing extra
- **⏭️ What You Skipped** — sarcastic summary of the fluff you escaped

## How to use

1. Open any food blog or recipe page
2. Click the extension icon
3. Hit **▶ Extract Recipe**
4. Get the recipe instantly — no scrolling required

## Setup

1. Load the extension in Chrome (`chrome://extensions` → Developer Mode → Load unpacked)
2. Click ⚙ and paste your [Gemini API key](https://aistudio.google.com/apikey)
3. Done — works on any recipe page

## Tech

- Chrome Extension Manifest V3
- Google Gemini API (with OpenRouter fallback)
- Two-phase loading: instant word count preview → full recipe extraction

---

Built by [@happy_ships](https://x.com/happy_ships) · Day 4/180
