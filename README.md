## Hi, I'm Sheldon

I build data projects end to end: collecting the data, modelling it, testing it, and keeping it running without me watching.

### Featured project: [UFC Fight Predictor](https://github.com/slixz7/ufc-project)

A web app that predicts UFC fights **before they happen**, locks every pick with a timestamp, explains it in plain language, and grades itself in public.

- **Live app:** https://ufc-predictor.streamlit.app/
- **Honest results:** in a backtest of 5,279 fights, the market-informed model picks 65.4% correctly against 61.8% for my statistics-only model and 64.9% for the bookmakers' opening line alone. The market does most of the work, and the project says so. The live record (37 of 52) is far too small to prove anything.
- **Runs unattended:** a daily GitHub Actions job loads cards, betting lines and results, locks picks and grades finished events, with a watchdog, outside heartbeats and weekly backups to catch anything that quietly stops.
- **Tested:** 1,094 offline tests, including checks that run against a real Postgres server on every push.
- **Read more:** [the write-up](https://github.com/slixz7/ufc-project/blob/main/docs/writeup.md), including the result that was too good to be true.

**Built with:** Python (pandas, scikit-learn), PostgreSQL (Neon), SQL window functions, Streamlit, GitHub Actions.
