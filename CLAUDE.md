# Eldevesland Wiki — CLAUDE.md

## What this project is

This is the world wiki for **Eldevesland**, a homebrew D&D world created by David Bolivar. It is built with [Quartz v4](https://quartz.jzhao.xyz/) and **automatically published on every push** — there is no separate deploy step. Edit files, commit, push, and the wiki is live.

The content is written primarily in **Spanish**, as that is the language of the campaign and world.

## Deployment

```
git add <files>
git commit -m "..."
git push
```

That is the full deploy pipeline. No build commands needed locally — Quartz builds on the server. To preview locally:

```
npx quartz build --serve -d docs
```

## Repository layout

```
content/                    ← All wiki pages (Markdown)
  index.md                  ← World root page
  Eldevesland/
    Eldoria/                ← Primary continent (most content lives here)
    Valindra/               ← Mystical continent
    Zhor'Khaz/              ← Arid/militaristic continent
  Reglas de Juego/          ← D&D homebrew rules
quartz.config.ts            ← Site title, plugins, theme, base URL
quartz.layout.ts            ← Sidebar/header layout
quartz/                     ← Quartz framework source (do not edit)
```

## Content structure and conventions

### File naming

- Files use **full Spanish names with spaces** — do not slugify or rename to kebab-case.
- Folder names mirror the region/topic they represent, e.g. `Thalassia (Coalicion del Norte)/`.
- Index files for a region share the folder's name: `Eldoria/Eldoria.md`, `Zhor'Khaz/Zhor'Khaz.md`.

### Frontmatter

Keep frontmatter minimal. Only `title:` is required:

```yaml
---
title: Nombre de la Página
---
```

Do not add dates, tags, or aliases unless there is a specific reason.

### Internal links

Use Obsidian-style wikilinks. Both forms are used in the existing content — prefer the explicit path form for cross-folder links:

```markdown
[[content/Eldevesland/Eldoria/Thalassia (Coalicion del Norte)/Thalassia|Thalassia]]
[[Veridia]]
```

### Page structure

Follow the section pattern established in existing pages. Use bold headings (`**Sección:**`) for top-level fields on denser pages, and Markdown `###`/`####` headers for named subsections. For example:

- Continental overview pages: Descripción General → Geografía y Biomas → Razas → Cultura y Sociedad → Ciudades Principales → Rumores y Leyendas
- Noble house entries: Casa Name → Raza → Emblema → Descripción (Historia + Especialización + Residencia) → Características
- Race pages: overview → specializations/houses
- City pages: Líder → Descripción → Ubicaciones Importantes → Especialidad

Rumors and legends use blockquotes with an attribution:

```markdown
> **"Rumor text."** — Source (location)
```

## The world: Eldevesland

Eldevesland is a homebrew D&D world. The three main continents are:

### Eldoria (primary continent)

The most developed continent, with a turbulent history. Originally inhabited by elves and dwarves, humans grew in number and transformed it through magic and technology. Divided into:

- **Thalassia** (Coalición del Norte) — feudal, magic-heavy, 8 noble houses, capital Luminaris ruled by Emperador Arcano Eldrin Thalarius. Houses: Amarthir, Eldorath, Larethian, Valthoris, Faelivrin, Galevaris, Thandoril, Miralith.
- **Veridia** (Coalición del Sur) — formerly feudal, now governed by the Consejo de los Seis. No king. Commercial guilds and the Caballeros de Gaia hold political influence alongside nobles. Peasants vote for El Vocero del Pueblo (3 council votes). Noble families retain legal privileges through old laws nobody has managed to repeal. Capital Mythralis. Noble houses: **Casa Valdris** (Duques, formerly ruling family), **Casa Ferrath** (Condes, Ironcliff, military/mining), **Casa Sylvaine** (Condes, Valewood, forests), **Casa Brenhal** (Barones, Goldhaven, agriculture), **Casa Maren** (Baronesa, Dunmire, alchemy — newest, most progressive), **Casa Vorthen** (Barones, eastern frontier, despised toll collectors), **Casa Delmira** (Hidalgos, Mythralis, broke nobility with title but no land).
- **Gran Bosque de Lythrandor** (centre) — Forest Elves homeland, capital Elandor.
- **Mountains/southwest** — Mountain Dwarves and Rock Gnomes.
- **Aetheria** (northeast) — magical floating city, founded after a cataclysm; High Elves, humans, and engineer dwarves collaborating on magic and technology. Noble family: Dreamhide.

Races documented in `Razas/`: Altos Elfos, Elfos del Bosque, Enanos de montaña, Gnomos de la roca, Humanos Coalicion del Norte, Humanos Coalicion del Sur.

Religions documented in `Religiones Comunes/`: Gaia, Luminara, Moradin, Neroth, Sylvannis.

### Valindra

A mystical, magic-rich continent with stable peace. Society is deeply connected to nature and arcane arts. Independent kingdoms each with their own leader. Races: Dragonborns, Aarakocra, Aasimar, Genasi, Firbolgs, Kenku, Tabaxi, Tritones, Lizardfolk, Gith. Cities: Lunaris (Reina Seraphina, Cronomancy), Aquamara (Rey Triton), Skyreach (Emperador Aarak, floating), Pyraxis (Archidruida Ignis, volcano). Special subclasses: **Cronomancia** (secret meta-school of time magic) and **Dragonknights** (chosen once per century, dragon-heart blessed).

### Zhor'Khaz

Arid and challenging, a continent of deserts, fire mountains, and underground cavern networks. Known for dark magic, militarism, and mineral wealth. Races: Tieflings, Medio Orcos, Humanos, Enanos, Gnolls, Aasimar. Cities: Drakhor (fortress, military), Kharazad (trade hub, Sultan), Tormak, Refugio de Asmodia (Tiefling city, infernal pacts).

## Reglas de Juego

The `Reglas de Juego/` folder holds D&D homebrew rules used at this table. These are game mechanics, not lore, and should be written in practical terms (list format, clear conditions). Current rules: Combat Homebrew (stacking advantage/disadvantage, flanking, targeted attacks, opportunity attacks), Ataque de Oportunidad (detailed rules), Críticos con Perdida de Extremidades.

## Writing guidelines

- **Language:** Spanish for all lore and world content. English is acceptable for game mechanics if the source material is in English.
- **Tone:** Descriptive and immersive for lore pages. The world has political intrigue, ancient mysteries, and magic woven into everyday life.
- **Consistency:** Match the style of existing pages. If adding a new noble house, follow the Casa Name / Raza / Emblema / Historia / Especialización / Residencia / Características pattern exactly.
- **No invented facts:** Do not add lore, characters, places, or mechanics that haven't been established by the user. Ask before creating new canon.
- **Rumors section:** Great pages include a `**Rumores y Leyendas:**` section with 4–6 blockquote rumors that hint at deeper mysteries without confirming them.

## Quartz configuration notes

- `quartz.config.ts`: base URL is `quartz.jzhao.xyz`, locale `en-US`, analytics via Plausible. Plugins active: ObsidianFlavoredMarkdown, TableOfContents, CrawlLinks, LaTeX, GitHubFlavoredMarkdown, SyntaxHighlighting.
- `ignorePatterns`: `private`, `templates`, `.obsidian` — content in these folders is never published.
- Theme fonts: Schibsted Grotesk (headers), Source Sans Pro (body), IBM Plex Mono (code).
- Sidebar: Explorer + Graph + TableOfContents + Backlinks — structure your pages so the graph and backlinks are meaningful.
