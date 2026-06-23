# 🏥 Pharmacy Locator System

A complete pharmacy locator project for Addis Ababa that helps patients find the right pharmacy for their prescribed medicine, with location-aware search and pricing support.

## Overview

This repository contains a full-stack system with:
- A Flask backend for medicine search and pharmacy data access
- A machine learning model for smarter medicine matching
- A React/Vite frontend for search, results, and map display

## Key Features

- Search pharmacies by medicine name
- Filter pharmacy results by availability and price
- Display pharmacy details and locations
- Train and reuse a medicine matching model

## Project Structure

```text
pharmacy-locator/
├── backend/
│   ├── app.py                  # Main Flask app
│   ├── model.py                # ML model logic (medicine search)
│   ├── train_model.py          # Train & save the model
│   ├── data/
│   │   ├── Addis_ababa_pharmacy.csv
│   │   └── medicine_list_training.csv
│   ├── models/
│   │   └── medicine_model.pkl  # Saved trained model
│   └── requirements.txt
└── frontend/
    ├── src/
    │   ├── App.jsx
    │   ├── pages/
    │   │   ├── Home.jsx
    │   │   ├── Search.jsx
    │   │   └── Results.jsx
    │   ├── components/
    │   │   ├── PharmacyCard.jsx
    │   │   ├── SearchBar.jsx
    │   │   └── MapView.jsx
    │   └── api/
    │       └── axios.js
    ├── index.html
    ├── vite.config.js
    └── package.json
```

## Getting Started

### Backend

1. Open a terminal and navigate to the backend folder:
   ```bash
   cd backend
   ```
2. Create and activate a Python virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate
   ```
3. Install the backend dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the Flask app:
   ```bash
   python app.py
   ```

### Frontend

1. Open a terminal and navigate to the frontend folder:
   ```bash
   cd frontend
   ```
2. Install frontend dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Notes

- The backend uses `backend/data/` for CSV data and `backend/models/` for the trained model.
- Run `backend/train_model.py` if you want to retrain or update the saved medicine matching model.
- Update frontend API settings in `frontend/src/api/axios.js` as needed to match the backend URL.

## License

