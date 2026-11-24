# DDI v2 forecast receipts

Public, time-stamped copies of the DDI v2 Fantasy Premier League forecasts, saved before each gameweek deadline. The commit times show when each forecast was made.

Each gameweek has a folder, `forecasts/gwNN/`:

| File | What it holds |
|---|---|
| `model.csv` | A: the DDI v2 model's expected points for the gameweek (xP1), for every player |
| `h.csv` | H: the same forecast with its spread shrunk, by position |
| `last5.csv` | F: each player's average points over their club's last five gameweeks (a simple baseline) |
| `saved.json` | When the forecast was saved, the deadline, and whether it was made on provisional data (the previous gameweek's points not yet final) |

Forecasts are saved by every scheduled run in the 24 hours before a deadline. A later save replaces an earlier one, and the commit history keeps every version. Nothing is written once the deadline is under ten minutes away.

Results and scoring: [andrewdeighan.com](https://andrewdeighan.com).
