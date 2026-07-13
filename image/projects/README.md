# Project screenshots

Drop a screenshot for each project here using the exact filenames below. The cards
on `index.html` show a dashed "screenshot: <name>.png" placeholder until the image exists.

Any media marked with `has-image` (single screenshot or image/video toggle) is
automatically enlargeable: click the thumb to open a centered lightbox; click the
dimmed sides or press Escape to return to the grid. No extra JS needed for new cards.

## How to make an image appear on a card

1. Add the file to this folder (e.g. `byow.png`).
2. In `index.html`, find that project's `.project-thumb` and turn on the image:

```html
<div class="project-thumb has-image" style="background-image:url('image/projects/byow.png')">
  <span class="thumb-label">screenshot: <span>byow.png</span></span>
</div>
```

The `has-image` class hides the placeholder label and grid overlay; the label can stay
in the markup as a fallback. Clicking the thumb opens the enlarge lightbox.

Recommended size: 16:9, at least 640x360 (1280x720 looks crisp on retina).

## Image + video toggle (optional)

For a screenshot/video carousel on one card, use `media-toggle` with stacked
`.thumb-media` elements. Side arrows and a video timeline are injected automatically;
enlarge still works on whichever slide is active:

```html
<div class="project-thumb has-image media-toggle">
  <img class="thumb-media active" src="image/projects/example.png" alt="Example screenshot">
  <video class="thumb-media" src="image/projects/example.mp4" muted loop playsinline preload="metadata"></video>
</div>
```

- Hover the thumb to reveal ‹ › arrows (always visible on mobile)
- When a video slide is active, a seekable progress bar + `current / duration` appears at the bottom
- Click the media itself to enlarge; click the dimmed sides or press Escape to close

## Expected filenames

Foundations & Data
- `ants.png` — Ants vs. SomeBees (CS 61A)
- `ants.mp4` — Ants vs. SomeBees gameplay clip (arrow-toggle with the screenshot;
  convert a .mov with
  `ffmpeg -i ants.mov -vcodec h264 -an -movflags +faststart ants.mp4`)
- `byow-1.png`, `byow-2.png` — Build Your Own World screenshots (CS 61B)
- `byow.mp4` — Build Your Own World gameplay clip (third slide on the card's arrows)
- `poverty-map.png` — Global Poverty Analysis (Data 8)
- `climate-change.png` — Climate Change Analysis (Data 8)
- `movie-classifier.png` — Movie Genre Classifier (Data 8)

Systems & Security
- `exploits.png` — Memory Safety Exploitation (CS 161)
- `pintos.png` — Pintos Operating System (CS 162)
- `http-server.png` — Multithreaded HTTP Server (CS 162)
- `mapreduce.png` — Distributed MapReduce (CS 162)
- `shell.png` — Unix Shell (CS 162)
- `allocator.png` — Kernel Heap & Allocator (CS 162)

Networking
- `tcp.png` — TCP Transport Protocol diagram (CS 168)
- `tcp.mp4` — TCP Transport Protocol demo clip (arrow-toggle with the screenshot)
- `routing.png` — Distance-Vector Routing (CS 168)
- `routing.mp4` — Distance-Vector Routing demo clip (arrow-toggle with the screenshot)
- `traceroute.png` — Traceroute Utility (CS 168)

AI & Machine Learning
- `pacman-ai.png` — Pacman Search & Adversarial AI (CS 188)
- `pacman-ai.mp4` — Pacman Search & Adversarial AI gameplay clip (arrow-toggle with the screenshot)
- `rl-agents.png` — Reinforcement Learning Agents (CS 188)
- `ghost-tracking.png` — Bayesian Ghost Tracking (CS 188)
- `neural-nets.png` — Perceptrons to Transformers (CS 188)
- `deep-learning1.png`, `deep-learning2.png` — Deep Learning & Fine-Tuning (CS 189)
- `autodiff.png` — Autodifferentiation Engine (CS 189)
