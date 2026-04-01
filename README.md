# BuddyDex

**[Live Demo](https://shipitandpray.github.io/buddy-dex/)**

Pokedex-style completion tracker for Claude Code `/buddy` species. Gotta discover 'em all.

## What is this?

Track which of the 18 buddy species (+ 18 shiny variants = 36 total) you've encountered. Enter friend's usernames to "discover" new species. No single person can complete the dex alone — you need to trade usernames with friends.

## Features

- **Your Buddy** — Register your username to see your own buddy
- **Discovery Grid** — 36 slots (18 species + 18 shiny variants) with ASCII sprites
- **Discovery Animation** — Flash + "NEW!" badge when you find a new species
- **Species Details** — Click any slot to see stats, lore, and rarity info
- **Completion Tracker** — Progress bar and percentage
- **Trophy Case** — 12 achievement badges for milestones
- **Share Card** — Generate a summary image of your dex progress
- **Challenge Hints** — Tips to help you find missing species
- **Persistent** — All progress saved in localStorage
- **Mobile Responsive** — Works on all screen sizes

## How it works

Every username deterministically maps to one of 18 species via Mulberry32 PRNG + hash function (same algorithm as the real `/buddy`). Species have different rarity tiers and a 1% chance of being shiny.

## Tech

Single `index.html` file. Zero dependencies. Uses Canvas API for share card generation.

## License

MIT
