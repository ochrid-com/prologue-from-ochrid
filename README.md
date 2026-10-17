# The Prologue from Ochrid — English

St. Nikolai Velimirovich's *Prologue from Ochrid*, translated into English directly from the original Serbian by Marcian Sakarya, [OCHRID.COM](https://ochrid.com). 366 days.

## License

[Creative Commons Attribution-ShareAlike 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use, copy, adapt and redistribute freely, including in apps, as long as you:

- credit **Marcian Sakarya** and **OCHRID.COM** with a link to https://ochrid.com, and
- release adapted versions of the text under the same license.

Suggested attribution: *"The Prologue from Ochrid, translated by Marcian Sakarya, OCHRID.COM (https://ochrid.com), CC BY-SA 4.0."*

## Dates

Files are keyed by the **Julian (Old Calendar)** date, as in the original book. `date_gregorian` gives the corresponding civil date for the 20th–21st centuries (+13 days). `02-29` exists for leap years.

## Contents

- `markdown/MM/MM-DD.md` — one file per day. Sections: `## Lives of the Saints` (each saint under `###`), `## Hymn of Praise`, `## Reflection`, `## Contemplation`, `## Homily`. Hymn line breaks are Markdown hard breaks (two trailing spaces).
- `prologue.json` — all days in one file, same text split into fields:

```json
{
  "date_julian": "01-01",
  "date_gregorian": "01-14",
  "title": "...",
  "lives": [{ "heading": "...", "text": "..." }],
  "hymn": "...",
  "reflection": "...",
  "contemplation": "...",
  "homily": "..."
}
```

Text fields are Markdown.

## Getting the data

```sh
git clone https://github.com/ochrid-com/prologue-from-ochrid.git
```

Corrections land continuously. Run `git pull` from time to time to stay current.

Generated 2026-10-17.
