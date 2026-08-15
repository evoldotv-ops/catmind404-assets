# catmind404-assets

Öffentliche Ablage für die Thumbnails des YouTube-Kanals **Cat Mind 404**
(@thecatmind404). Das Repo existiert nur, weil YouTube das Thumbnail beim Upload
**selbst über eine öffentliche URL abholt** — es lässt sich nicht direkt
mitschicken.

Kein Code, keine Rohdateien, keine Skripte.

## URL-Muster

```
https://raw.githubusercontent.com/evoldotv-ops/catmind404-assets/main/thumbnails/<ordner>.jpg
```

`<ordner>` ist der Ordnername aus `D:\Katzenkanal\_upload`, z. B.
`01_the-red-dot`. Alle acht Folgen liegen hier.

## Verwendung beim Upload

```
youtubeThumbnailUrl: "<Thumbnail-URL>"
```

Am 15.08.2026 gegen einen privaten Testupload geprüft: `"thumbnail_set": true`.

## Warum hier keine Untertitel liegen

`youtubeSubtitles` in `upload-post` wird von YouTube **nicht übernommen**. Der
Testupload (Video `TzzxtAGlkhI`) hatte im Studio nur den automatisch erzeugten
Track, unsere SRT tauchte nicht auf. Die Antwort der API meldet dazu weder
Erfolg noch Fehler — es gibt für Untertitel überhaupt kein Feld.

Die fertigen SRTs liegen deshalb nur lokal in
`D:\Katzenkanal\_upload\<ordner>\untertitel.srt` und werden bei Bedarf von Hand
im Studio hochgeladen. Sie enthalten den kompletten Sprechtext einer Folge und
haben auf einer öffentlichen Seite ohnehin nichts verloren.

## Achtung: raw-CDN cacht

Eine geänderte Datei kam unter derselben URL über zwei Minuten lang in der alten
Fassung zurück, auch mit Cache-Buster-Parameter. Wer ein Thumbnail austauscht,
lädt es unter **neuem Dateinamen** hoch. Und Assets ein paar Minuten vor dem
Upload pushen, nicht in derselben Minute.
