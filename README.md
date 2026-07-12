# The Football Field Guide

A friendly, interactive introduction to football concepts for sharing with family and friends.

**Live site:** https://jewelshovan.github.io/football-concepts-learning/

## What is included

- A four-picture **Match Reader** that teaches learners to look away from the ball, commit to a read, and then reveal the tactical cue.
- An interactive expected-goals (xG) pitch plus a categorical chance builder and 100-shot simulation.
- Pressing, decision-making, offside, and team-identity interactives.
- A first-five-seconds transition lab and phase-based formation explorer showing how the same players’ jobs change with and without the ball.
- Plain-English explanations and quizzes for xG, xA, PPDA, possession, and changing game-state context.
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
