# Pokémon Lab

Pokémon Lab is a vanilla HTML/CSS/JavaScript Pokémon companion application built by upgrading the existing Pokémon Card Lab project rather than introducing a new framework.

## Included
- Home dashboard with Pokémon of the Day, collection progress, quick actions, daily challenge and recently viewed
- Search Pokémon by name/ID
- Universal search with type, generation and category routing plus ability/move lookup fallback
- Search by Type with all results loaded progressively
- Detailed Pokémon Info / evolution family research
- Full Pokémon research modal: stats, abilities, moves, forms, cry, weaknesses/resistances and evolution chain
- My Collection with add/remove, favorites, shiny tracking, filters, sorting and grid/list view
- Advanced search by generation, type, category and stats
- Favorites
- Shiny Collection
- Team Builder for up to six Pokémon, saved teams, reorder controls and coverage analysis
- Pokémon comparison for 2–4 Pokémon
- Interactive Type Effectiveness Lab and type matrix
- Stat Calculator
- Simplified Damage Calculator
- "What Beats My Pokémon?" weakness analyzer
- Simplified Quick Battle with moves, damage, HP and battle history
- Mystery Card 2.0 with random discoveries, rarity categories and optional shiny draws
- Who's That Pokémon? quiz modes: silhouette, multiple choice, type, evolution and stat
- Pokémon Cry Quiz using cries exposed by the API
- Daily challenges
- Trainer profile, XP/levels and achievements
- Regions explorer
- Personal analytics
- Light / Dark / System themes and reduced-motion setting
- Responsive desktop/tablet/mobile navigation
- Loading, empty and error states
- Local persistence for collection, favorites, shiny tracking, teams, trainer, XP, quiz stats, battle history, mystery history, recent views and theme

## Run
No build step or package installation is required.

Open `index.html` in a browser, or serve the folder with any static HTTP server.

Example:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000/`.

## Data source
The app uses the public PokéAPI (`https://pokeapi.co/api/v2/`). No private API key is required.

## Limitations
- This project has no backend/authentication; trainer data is intentionally stored in localStorage.
- Battle and damage calculations are explicitly simplified estimates and are not a replacement for the official game battle engine.
- Pokémon TCG card data is not fabricated; Mystery Card uses Pokémon data from PokéAPI and labels rarity as a Lab/game category.
- Advanced category filters such as Starter/Fossil/Paradox use small local classification lists where PokéAPI does not expose a universal category field.
- Large searches are intentionally loaded in batches to reduce API pressure.
- Cry playback depends on the cry URL being available and browser audio permissions.
