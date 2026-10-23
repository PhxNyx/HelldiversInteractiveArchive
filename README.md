# Democracy Archive

**An interactive, Super Earth–flavoured companion to the Helldivers 2 wiki.**

Democracy Archive recreates the community wiki as a single, fast, installation-free web app: browse every enemy, weapon and stratagem, build and rate a loadout, track the Major Orders, and turn your own career statistics into a shareable Combat Record card. The whole experience is presented as official Ministry of Truth material, tongue firmly in cheek.

**[Open the live site](https://phxnyx.github.io/HelldiversInteractiveArchive/)**

> Unofficial fan project. See [Disclaimer](#disclaimer).

---

## Features

| Section | What it does |
| --- | --- |
| **Headquarters** | Live war counters and a quick way into every section. |
| **Timeline · Lore · Factions** | The history of Super Earth, its factions and its universe, with a briefing for each entry. |
| **Bestiary** | Every Terminid, Automaton and Illuminate unit, with data read from the wiki. |
| **Galaxy** | An interactive map of the galaxy. |
| **Major Orders** | The complete history of Major Orders, with outcomes and statistics. |
| **Armory** | Weapons, armor and equipment, with their wiki stats. |
| **Loadout Builder** | Pick or roll a full loadout, lock your favourites, get an evaluation by front (Terminids, Automatons, Illuminate) and export it as an image. |
| **Stratagems** | An arrow-code simulator to practise stratagem inputs. |
| **XP Calculator** | How much XP separates two levels, with a progression chart. |
| **Titles** | The full rank ladder, every Warbond and special title, and a printable Service Record. |
| **Combat Record** | Enter your career statistics and get analytics, a rating, a doctrine, commendations and a printable card. |
| **Duel** | Compare two Combat Records side by side, with a verdict and a shareable image. |
| **Warbonds** | Every Warbond page and its full contents. |
| **Changelog** | Patch notes and an update report. |
| **Glossary · Loyalty Exam** | The official vocabulary, and a quiz to test your devotion. |

Also included: archive-wide search, a mobile-friendly navigation drawer, and PNG export for loadouts, Combat Records and Duels.

### Combat Record

The game records a lot of career statistics but shows them as plain lists. Combat Record turns them into something readable:

- **Derived metrics**: K/D ratio, accuracy, shots per kill, kills and deaths per mission, kills per hour, win and extraction rates, XP per hour, friendly-fire rate and more.
- **Democracy Rating**: an unofficial grade from S to F, with a radar chart covering lethality, marksmanship, survival, missions, logistics and discipline.
- **Doctrine and commendations**: a play-style label and a set of milestone badges.
- **Breakdowns**: kills by front, kill methods and stratagem mix.
- **Export**: a ready-to-share PNG card, plus a plain-text summary.

Statistics are entered by hand. The game does not expose them through a public interface.

---

## Using it

Open the [live site](https://phxnyx.github.io/HelldiversInteractiveArchive/), or download `index.html` and open it in any modern browser. There is nothing to install and no build step.

The app works best with an internet connection, because most of the content is read live from the wiki. If the wiki cannot be reached, it falls back to data cached earlier in your browser.

### Privacy

- No account, no tracking, no analytics, no cookies.
- Everything you enter (callsign, statistics, loadouts, preferences) is stored **only in your browser** (`localStorage`) and never leaves your device.
- Exported images are generated locally in your browser. If the wiki's own images cannot be read directly, the public image proxy [wsrv.nl](https://wsrv.nl) may be used to fetch those wiki images; none of your data is sent along.

---

## Data sources

All game information comes from the community. Thank you to everyone who maintains it.

- **[Helldivers Wiki](https://helldivers.wiki.gg)** (wiki.gg): primary source for enemies, weapons, armor, stratagems, Warbonds, titles and levels. Text and images are available under [CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/) unless otherwise noted; every entry in the app links back to its wiki page.
- **[Helldivers Wiki on Fandom](https://helldivers.fandom.com)**: secondary source, used when the primary one is not available.
- **[Shacknews](https://www.shacknews.com)**: community-verified level table, used as a cross-reference for the XP Calculator.
- **[Helldivers Training Manual API](https://helldiverstrainingmanual.com)**: community-run public API for the live war counters and planet data.

---

## Technical notes

- A single self-contained HTML file: no framework, no dependencies, no bundler.
- Plain HTML, CSS and JavaScript. Developed and tested on Chromium-based browsers, on desktop and mobile; current versions of Firefox and Safari are expected to work as well.
- Hash-based routing, so every section has its own shareable URL (`#builder`, `#record`, and so on) and works on static hosting.
- Image export uses the Canvas API; no server is involved.

### Hosting on GitHub Pages

1. Name the file `index.html` and commit it to the root of the repository (or to `/docs`).
2. In **Settings → Pages**, choose the branch and folder to publish.
3. Open the URL GitHub shows you. Because the app is a single static file, no further configuration is needed.

---

## Contributing

Bug reports and suggestions are welcome through the repository's issue tracker. When reporting a problem, please include your browser and version, the section where it happened and, if possible, a screenshot.

Most game data comes from the wiki. If an entry is wrong or missing, the best fix is to correct it on the [Helldivers Wiki](https://helldivers.wiki.gg), and every user of the community benefits.

---

## Credits

Created and maintained by **Phenix**.

Game data courtesy of the Helldivers community wiki editors and the maintainers of the community API listed above.

---

## Disclaimer

Democracy Archive is an unofficial, non-commercial fan project. It is **not affiliated with, endorsed by or sponsored by** Arrowhead Game Studios or Sony Interactive Entertainment.

*Helldivers™* and *Helldivers™ 2*, and all related names, logos, characters and game assets, are trademarks and/or copyrighted works of their respective owners. They are used here for identification and commentary only. All propaganda in this project is fictional, and the Ministry of Truth assumes no responsibility for any loss of limbs, friends or personal freedoms.

*Spread Managed Democracy.*
