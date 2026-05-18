# Mad Cow Pro Team Value Dashboard

Bilingual internal team-value report for Mad Cow Basketball.

Public page: https://bayareamadcow.github.io/akila-vs-sean/

Repository: https://github.com/bayareamadcow/akila-vs-sean

## What This Is

This is not opponent scouting. It is an internal coach-facing usage report that explains:

- each player's strengths
- what each player should improve
- the best way to use each player
- team value and lineup fit
- best five-player lineups

中文版本：这是队内用人报告，不是对手 scouting。重点是每个人怎么用、怎么进步、在队里有什么价值，以及哪些阵容最适合赢球。

## Source Model

The website combines two inputs:

- `20-game film context`: used for role continuity, player habits, lineup fit, and decision-quality patterns.
- `8-game Pro score-sheet PDF`: used as the statistical anchor for points, PPG, made threes, scoring share, and lineup recommendations.

The Pro PDF is stored at:

`assets/reports/mad-cow-8-games-pro-coach-report.pdf`

## Current Best Five

`Yang #23`, `Willy #26`, `Eaxin #3`, `James #25`, `Akila #88/#69`

Why this lineup works:

- `Yang` creates the first pressure and brings real three-point gravity.
- `Willy` is the team-high shooter and keeps the floor spaced.
- `Eaxin` stabilizes the offense with midrange outlets and lower-risk decisions.
- `James` gives screens, rebounding, first contact, and frontcourt structure.
- `Akila` supplies top scoring production and offensive rebounding.

## Project Structure

- `index.html`: the public bilingual dashboard.
- `styles.css`: layout, visual system, responsive behavior.
- `assets/stills/`: player still images.
- `assets/reports/`: downloadable PDF source report.

## Local Preview

Run a static server from the repository root:

```powershell
python -m http.server 8123 --bind 127.0.0.1
```

Then open:

```text
http://127.0.0.1:8123/
```
