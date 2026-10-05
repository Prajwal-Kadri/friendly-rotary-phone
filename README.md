# Friendly Rotary Phone

Friendly Rotary Phone is a Flask web app that recommends a Codeforces problem for a user based on their recent submissions and preference.

## Features

- Accepts a Codeforces handle as input
- Supports two recommendation modes:
  - `1`: a problem similar to what the user already solves
  - `2`: a problem from less-practiced areas
- Returns one recommended problem

## Tech Stack

- Python
- Flask
- CodeforcesApiPy

## Project Structure

- `/flask_app.py` – main Flask application and recommendation logic
- `/templates/form.html` – input form UI
- `/static/` – styles and static assets
- `/IEP_data_save.data` – serialized recommendation data

## Getting Started

### 1) Clone the repository

```bash
git clone https://github.com/Prajwal-Kadri/friendly-rotary-phone.git
cd friendly-rotary-phone
```

### 2) Install dependencies

```bash
pip install -r requirements.txt
```

### 3) Run the app

```bash
python flask_app.py
```

The app starts on `http://127.0.0.1:5000` by default.

## Usage

1. Open the app in your browser.
2. Enter your Codeforces handle.
3. Enter preference:
   - `1` for likeable problem
   - `2` for useful problem
4. Submit the form to get a recommendation.

## Deployment

This repository includes a `Procfile`:

```text
web: python flask_app.py
```

It can be used for platform deployments that support Procfile-based process definitions.
