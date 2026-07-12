# The Football Field Guide

A friendly, interactive introduction to football concepts for sharing with family and friends.

**Live site:** https://jewelshovan.github.io/football-concepts-learning/

## What is included

- A persistent section navigator with all 13 learning stops, current-section highlighting, scroll progress, and a mobile-friendly menu.
- An interactive **Match Clock Decoder** covering regulation, added/stoppage time, extra time, penalty kicks, and penalty shoot-outs.
- A four-picture **Match Reader** that teaches learners to look away from the ball, commit to a read, and then reveal the tactical cue.
- An interactive expected-goals (xG) pitch plus a predict-before-reveal chance builder and animated 100-shot simulation.
- Pressing, decision-making, team-identity interactives, and a draggable offside lab with equivalent tap and keyboard controls.
- A first-five-seconds transition lab and phase-based formation explorer showing how the same players’ jobs change with and without the ball.
- Expandable stat cards for xG, xA, PPDA, xT, field tilt, progressive actions, and box entries.
- Animated scoreline contexts showing how the clock and score change the meaning of possession, shots, and xG.
- A three-round **Sofa Stats Huddle** for family and friends to interpret animated match comparisons together—without timers, scores, or leaderboards.
- A one-lens matchday mission and observation checklist saved locally in the browser.

The evidence-informed teaching rationale and development roadmap are documented in [`RESEARCH.md`](RESEARCH.md).

## Run locally

This is a dependency-free static site. Open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publishing

The included GitHub Actions workflow deploys every push to `main` to GitHub Pages. In the repository settings, select **Settings → Pages → Source: GitHub Actions** if it is not selected automatically.

The xG calculator is a teaching model based on shooting distance and the angle between the posts. It is deliberately not a claim to be a production or provider-grade xG model.
