# The Prologue from Ochrid — English

St. Nikolai Velimirovich's *Prologue from Ochrid*, translated into English directly from the original Serbian by Marcian Sakarya, [OCHRID.COM](https://ochrid.com). 366 days.

## License

[Creative Commons Attribution-ShareAlike 4.0](https://creativecommons.org/licenses/by-sa/4.0/). Use, copy, adapt and redistribute freely, including in apps, as long as you:

- credit **Marcian Sakarya** and **OCHRID.COM** with a link to https://ochrid.com, and
- release adapted versions of the text under the same license.

Suggested attribution: *"The Prologue from Ochrid, translated by Marcian Sakarya, OCHRID.COM (https://ochrid.com), CC BY-SA 4.0."*

## Dates

Files are keyed by the **Julian (Old Calendar)** date, as in the original book. `date_gregorian` gives the corresponding civil date for 1900–2099 (+13 days) in a **common year**.

Leap years shift the end of February. The Julian calendar has its own February 29, so in a leap year Julian `02-16` through `02-29` fall one day earlier than `date_gregorian` says: `02-16` is February 29, `02-28` is March 12 and `02-29` is March 13. From Julian `03-01` (March 14) on, the dates agree again. `02-29` exists only in leap years, so its `date_gregorian` is its leap-year date, `03-13`. Compute the date from the year if your app needs it exact.

## Translation status

`status` is `"translated"` (complete, but may include awkward phrases or minor issues) or `"verified"` (a close reading has been done for natural, hagiographic English). Text marked `translated` may still change.

## Contents

- `markdown/MM/MM-DD.md` — one file per day. Sections: `## Lives of the Saints` (each saint under `###`), `## Hymn of Praise`, `## Reflection`, `## Contemplation`, `## Homily`. Hymn line breaks are Markdown hard breaks (two trailing spaces).
- `prologue.json` — all days in one file, same text split into fields:

```json
{
  "date_julian": "01-01",
  "date_gregorian": "01-14",
  "title": "...",
  "status": "verified",
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

Corrections land continuously. Run `git pull` from time to time to stay current. To be notified of changes, including days moving from `translated` to `verified`, subscribe to the commit feed in any RSS reader: https://github.com/ochrid-com/prologue-from-ochrid/commits/main.atom

Generated 2026-11-16.
