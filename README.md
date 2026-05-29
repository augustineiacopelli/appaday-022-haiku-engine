# App 022 · Haiku Engine

A haiku generator powered by the Claude API. Enter any topic or mood — morning fog, grief, a long flight home — and receive an original 5-7-5 haiku with a short reflection on the imagery choices that shaped it.

## How to Use

1. Type a topic or mood into the input field and tap **Compose**
2. The haiku appears line by line, followed by a brief commentary on its imagery
3. Tap **Send by Email** to open a pre-filled email to any recipient
4. Tap **Compose Another** to reset and write a new one
5. Tap the gear icon to open Settings and save your API key and default email address

## Technical Notes

- Vanilla HTML, CSS, and JavaScript — no frameworks or dependencies
- Calls the Anthropic Claude API directly from the browser using the `anthropic-dangerous-direct-browser-access: true` header
- API key and default email are stored in `localStorage` and persist across sessions
- The Claude prompt enforces strict 5-7-5 structure with concrete imagery requirements and returns structured JSON
- Email is sent via `mailto:` — opens the device's native mail app with the haiku pre-loaded

## Definition of Complete

- [x] Accepts a topic or mood as input
- [x] Returns a valid 5-7-5 haiku via Claude API
- [x] Displays haiku with staggered line-by-line animation
- [x] Includes imagery commentary below the haiku
- [x] Settings panel stores API key and default email persistently
- [x] Email modal pre-fills recipient and composes a ready-to-send message
- [x] Mobile-friendly at 375px viewport
- [x] Published to GitHub Pages
