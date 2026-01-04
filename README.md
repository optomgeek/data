## Data logging rules (5 lines)
1) JSONL logs are append-only: 1 line = 1 weekly record (Perth).
2) Every record must include `week_end_perth` (Sunday) and `period_perth.start/end`.
3) X sentiment goes to `data/x_sentiment_log.jsonl`; market homework goes to `data/market_data_log.jsonl`.
4) Keep keys snake_case and keep units explicit (pct, bp, close); add `data_quality_flags` if needed.
5) If a past record needs correction, append a new line with a note instead of editing history.
