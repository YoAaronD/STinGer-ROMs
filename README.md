# STinGer-ROMs

A MiSTer Downloader database listing exactly the ROM zips that [STinGer](https://github.com/YoAaronD/STinGer-Installer)'s games use, and nothing else.

It doesn't host any ROMs. Each entry points at the same archive.org files that Update All's Arcade ROMs database, Ongo and decoryah already use, so every zip carries the same name and hash as theirs. STinGer's own database only lists games. The ROM list lives here, separately, so you can keep it, swap it or drop it without touching the menu.

The full STinGer install already includes it. To add it by hand, put this in `downloader.ini`:

```
[YoAaronD/STinGer-ROMs]
db_url = https://raw.githubusercontent.com/YoAaronD/STinGer-ROMs/main/db.json.zip
filter = all
```

That's about 2.2 GB. The Cave CV1000 games need Raki's CV1000 core from [his Patreon](https://www.patreon.com/cw/ikamusume). If you'd rather leave them out, use `filter = !cv1000` here and in STinGer's section.

Bringing your own ROMs? Leave this section out.

The list is rebuilt from STinGer's game list; the per-game report is in [STinGer's docs/ROMS.md](https://github.com/YoAaronD/STinGer-Installer/blob/main/docs/ROMS.md).
