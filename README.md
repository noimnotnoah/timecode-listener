# timecode-listener

Hear timecode. A single-page web app that plays one short, high-pitched
click per frame so you can physically hear how fast a timecode is running.

Set the frame rate with one of the common presets (23.976, 24, 25, 29.97,
30, 50, 59.94, 60 fps) or type a custom rate, hit Start, and listen — at
24fps you'll hear 24 evenly spaced clicks per second, at 30fps you'll hear
30, and so on. The first frame of every second is accented (louder, higher
pitch) so you can also hear the second boundaries.

Built with plain HTML/CSS/JS and the Web Audio API's look-ahead scheduler
for sample-accurate timing (not `setInterval`, which drifts). No build
step, no dependencies — just open `index.html`, or use the GitHub Pages
deployment.

## Run locally

Open `index.html` directly in a browser, or serve the folder:

```
python3 -m http.server
```

## Live site

Deployed automatically via GitHub Actions to GitHub Pages.
