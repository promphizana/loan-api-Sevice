# Loan Prediction API

FastAPI service that returns a default-risk prediction for a loan application.

- `POST /predict`: body `{"amount_usd": 1500, "term_months": 12, "monthly_income_usd": 400}`
- `GET /health`: health check
- `/docs`: interactive documentation
- The model file is read from `MODEL_PATH` (default `model/model.json`).

Run with Compose: `docker compose up -d --build`
Run tests: `pip install -r requirements-dev.txt && pytest`
