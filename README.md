# Organ Donation: Transplant Viability and Recovery

A Django web application prototype for organizing donor, patient, doctor, and administrator workflows. It also includes experimental modules for estimating donor suitability, transplant outcomes, and recovery time.

> **Disclaimer:** This is an educational prototype, not a medical device. Its demo predictions are not clinically validated and must not be used to make medical, transplant, or treatment decisions. Do not use real patient or donor data.

## Features

- Separate registration and login pages for donors, patients, and doctors
- Administrator dashboard and account pages
- Donor and patient profile workflows
- Admission and support-ticket pages
- Experimental donor-suitability and transplant-outcome estimates
- Django models and stored prediction-model artifacts

## Technology

- Python and Django
- MySQL
- scikit-learn and joblib components for experimental prediction functionality

## Project layout

```text
myproject/
├── base/                 # Main application, models, views, and templates
├── ml_engine/            # Prediction-related code and model artifacts
├── myproject/            # Django project configuration
└── manage.py             # Django management command entry point
```

## Run locally

1. Install a Python version compatible with the Django version used by the project, then install the required packages.
2. Configure a local MySQL database and update the database and email settings for your environment. Keep passwords and Django secret keys out of source control; move them to environment variables before sharing or deploying.
3. From the `myproject` directory, run:

   ```bash
   python manage.py migrate
   python manage.py runserver
   ```

4. Open `http://127.0.0.1:8000/` in your browser.

## Data and security

Do not commit credentials, local database files, virtual environments, cache files, or real personal or health information. Use synthetic data for development and testing. Review Django’s deployment security checklist before deploying this prototype.
