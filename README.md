# PONG / Court 01

A self-contained arcade game built with HTML Canvas, CSS, and vanilla JavaScript.

## Play locally

Double-click `index.html`. No install, server, account, or internet required.

## Publish with GitHub Pages

1. Create a GitHub repository named `pong-game` (public works with GitHub Free).
2. Upload the extracted files to its root, with `index.html` at the top level. Do not upload the ZIP itself.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select **main** and **/(root)**, then **Save**.
6. Wait for deployment; GitHub displays your published link in Pages settings.

Your address follows `https://YOUR-USERNAME.github.io/pong-game/`.

Official publishing instructions: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Controls and rules

- Solo: W/S, Up/Down, mouse movement over the court, or touch and drag.
- Two players on the same device: player 1 W/S; player 2 Up/Down. On a touchscreen, each player drags their own half of the court.
- Space: start, pause, resume, or rematch when focus is on the court. Buttons work with Enter/Space; selects retain normal keyboard behavior.
- First to the selected score wins. Paddle edges return the ball at sharper angles. Each return increases speed to a cap.
- Easy, Normal, and Hard change the computer's speed, reaction time, and aim error.
- Restart returns to the ready screen. Changing mode, difficulty, or target score resets the match.
- Switching tabs/windows automatically pauses play. Resume manually.
- Sound starts off and can be enabled using the sound button.

## Embed on another website

Replace the URL with your published GitHub Pages URL:

```html
<iframe src="https://YOUR-USERNAME.github.io/pong-game/"
        title="Pong arcade game" width="100%" height="950"
        style="border:0;border-radius:10px" loading="lazy"></iframe>
```

## Files and customization

Everything needed to play is in `index.html`, including styles, physics, controls, computer opponent, and generated audio. There are no external fonts, images, trackers, APIs, or packages. `.nojekyll` bypasses Jekyll processing on Pages. Change the CSS variables near the top to adjust the palette. Game constants are near the start of the script.

The canvas playfield is visual; it is not a screen-reader-playable game. Buttons and settings are keyboard accessible, and scores are announced as points are earned. Multiplayer is local, not online.
