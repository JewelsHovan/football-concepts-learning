# The Football Field Guide

A friendly, interactive introduction to football concepts for sharing with family and friends.

**Live site:** https://jewelshovan.github.io/football-concepts-learning/

## What is included

- An interactive expected-goals (xG) pitch: move the ball and take a probability-based shot.
- Plain-English explanations of xG, xA, PPDA, and goal difference.
- A worked example showing why the scoreline does not tell the whole story.
- Simple lenses for watching possession, pressing, and player roles.

## Run locally

This is a dependency-free static site. Open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publishing

The included GitHub Actions workflow deploys every push to `main` to GitHub Pages. In the repository settings, select **Settings → Pages → Source: GitHub Actions** if it is not selected automatically.

The xG calculator is a teaching model based on shooting distance and the angle between the posts. It is deliberately not a claim to be a production or provider-grade xG model.
