# Birthday Film 2077

Static site for Tanish's birthday film. Hosted on GitHub Pages.

## Add the film

Drop your After Effects export at the repo root as `film.mp4` (1920 x 1080, H.264, music baked in), then:

```sh
git add film.mp4
git commit -m "Add film"
git push
```

GitHub rejects single files over 100 MB. If the export is bigger, either re-encode it smaller (e.g. `ffmpeg -i in.mp4 -c:v libx264 -crf 23 -preset slow -c:a aac -b:a 160k film.mp4`) or track it with Git LFS before committing.

## Fill in the blanks

In `index.html`, replace the three `[...]` placeholders inside `<span class="slot">`:

- the closing note
- the music credit
- the month and year
