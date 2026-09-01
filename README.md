# Comsect1 Themes

This repository is the data authority for portable semantic UI themes consumed
by Gantry and other Comsect1 applications. A theme supplies inert presentation
values only. It cannot name commands, executable paths, candidates, network
locations, trust material or runtime hooks.

`catalog.json` is the maintained catalog. Applications validate it against
`schema/theme-catalog.schema.json`, select only known semantic roles and retain
at most one local theme identifier. A missing catalog, invalid catalog or saved
identifier that no longer exists falls back to the consumer's one compiled
neutral theme.

Themes may be added or removed by editing `catalog.json`; consumers must not
hardcode the catalog. The maintained set currently includes Lemon, Hatbit,
Pitch, Melon, Water-melon, Sphaire, Emerald, Ruby, Diamond, Perl, Dalbit,
VSCode Dark, VSCode White and Windows 98. The user-facing spellings are catalog
data and consumers must preserve them.

## Semantic roles

- `canvas`, `sidebar`, `workspace`, `surface`, `raised`
- `text`, `muted`, `line`
- `accent`, `accentSecondary`, `onAccent`
- `success`, `warning`, `failure`, `focus`

All colors use exact `#rrggbb` notation. Layout, typography, motion and widget
behavior remain consumer responsibilities.
