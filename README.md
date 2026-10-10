# LindaLuna site

Website of SmartHeal LindaLuna, Luna's Parcours and Luna's Journey: https://lindalunawow.github.io

## How to change the site

Do not edit `en/`, `fr/`, `it/` or the root `index.html` by hand: they are generated and get overwritten.

1. Edit the English source: `src/site.en.html`.
2. For every English text you add or change, add or update its Italian and French version in the table `T` in `tools/build_i18n.py` (one row: English, Italiano, Français). The build stops if an English text in the table is missing from the source.
3. The language entrance page is `src/splash.html`.
4. Build from the repository root:

   ```
   python3 tools/build_i18n.py
   ```

5. Commit and push. GitHub Pages publishes in about a minute.

## Rules

- No details that change often: no quest counts, data dates, versions or per-level tables. Those belong in the CurseForge descriptions and changelogs.
- CurseForge links only for approved projects (`LINKS` at the bottom of `src/site.en.html`); the others show "Coming soon on CurseForge".
- No donation requests inside the addons (Blizzard policy); the PayPal link lives here and on CurseForge.
- Luna's farewell, *Might Luna guide you forward, always*, stays in English in every language.

## Images

Images are in `assets/` as `.webp`. Give a changed image a new file name so browsers don't show the cached one.
