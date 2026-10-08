# Codeforces Problem Recommender

A Flask application that recommends a Codeforces problem using a contestant’s submission history and a preference for familiar or less-explored problem groups.

## How it works

1. The user submits a Codeforces handle and preference.
2. The app retrieves recent submissions through the Codeforces API.
3. It compares solved problems with the stored problem groups.
4. It returns a randomly selected recommendation from the chosen group.

## Run locally

```bash
python -m pip install -r requirements.txt
python flask_app.py
```

Then open the local URL shown by Flask.

## Project structure

- `flask_app.py` — web app and recommendation logic
- `templates/form.html` — input form
- `IEP_data_save.data` — serialized problem-group data
- `static/` — styles and image assets
