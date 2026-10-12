# CSOP ETP Product Line — Interview Draw

A single-file, zero-dependency web app for randomly drawing one CSOP ETP / L&I
product (Ticker + Fund name) for interview questions.

- Draws **one** product at a time (Ticker + Fund name)
- **No repeats** — drawn items leave the pool
- **Start** → full-screen ticker randomly flashing → **Pause** stops and shows the draw
- **Reset** to restart; **Done** when all are drawn
- A **History** panel logs every draw
- Data sourced from CSOP PRODUCTS (ETF + L&I), excluding Mutual Fund
- Fully self-contained: data and logo embedded inline, no external requests

This page is published via GitHub Pages and works on any device / any network.

## Update the product list
Edit the source Excel and re-run `build_quiz.py` (in the parent project), then
copy the regenerated `etf-quiz.html` over `index.html` and push.

## Local preview
Open `index.html` directly, or run a static server:
`python -m http.server` then visit `http://localhost:8000`.
