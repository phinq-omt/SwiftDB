# Homepage frames

The homepage crossfades three WebP frames of the Lumen Atelier sample database. The files are 2160×1350.

| File | What it shows |
| --- | --- |
| `home/orders.webp` | The `orders` table, with the sidebar open. This is also the social preview image. |
| `home/query.webp` | A SQL query and its formatted results. |
| `home/palette.webp` | The command palette over that query. |

`index.html` cycles them over 12 seconds. `prefers-reduced-motion` keeps `orders.webp` still.

The sample data is `Scripts/Demo/lumen.sql`. Rebuild the SQLite file with:

```sh
sqlite3 Scripts/Demo/Lumen.sqlite < Scripts/Demo/lumen.sql
```

Serve the site locally with:

```sh
python3 -m http.server 8000 --directory docs
```
