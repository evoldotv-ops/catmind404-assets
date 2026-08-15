# catmind404-assets

Öffentliche Ablage für Thumbnails und Untertiteldateien des YouTube-Kanals
**Cat Mind 404**. Das Repo existiert nur, weil YouTube beide Dateiarten beim
Upload **selbst über eine öffentliche URL abholt** — sie lassen sich nicht
direkt mitschicken.

Kein Code, keine Rohdateien, keine Skripte. Nur die Dateien, die der Upload
braucht.

## URL-Muster

```
Thumbnail:   https://raw.githubusercontent.com/evoldotv-ops/catmind404-assets/main/thumbnails/<ordner>.jpg
Untertitel:  https://raw.githubusercontent.com/evoldotv-ops/catmind404-assets/main/untertitel/<ordner>.srt
```

`<ordner>` ist der Ordnername aus `D:\Katzenkanal\_upload`, z. B.
`01_the-red-dot`.

## Verwendung beim Upload

```
youtubeThumbnailUrl: "<Thumbnail-URL>"
youtubeSubtitles:   [{ language: "en", name: "English", url: "<Untertitel-URL>" }]
```

## Stand

| Folge | Thumbnail | Untertitel |
|---|---|---|
| 01 the-red-dot | ✓ | ✓ |
| 02 nothing-is-fun-anymore | ✓ | folgt vor dem Upload |
| 03 the-plan-dies-by-morning | ✓ | folgt vor dem Upload |
| 04 the-other-bowl | ✓ | folgt vor dem Upload |
| 05 snow-over-the-footprints | ✓ | folgt vor dem Upload |
| 06 the-doorway | ✓ | folgt vor dem Upload |
| 07 paid-for-the-chase | ✓ | folgt vor dem Upload |
| 08 never-on-you | ✓ | folgt vor dem Upload |

Die Untertiteldateien enthalten den kompletten Sprechtext einer Folge. Sie
werden deshalb erst kurz vor dem jeweiligen Upload hier abgelegt, damit nicht
acht unveröffentlichte Skripte gleichzeitig öffentlich stehen.
