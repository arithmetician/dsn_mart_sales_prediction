DSN Mart Sales Prediction — Bootcamp Qualification Hackathon 2026

A regression pipeline built for the DSN Bootcamp Qualification Hackathon 2026 (ML Track), hosted on Kaggle as part of Data Science Nigeria's selection process for the DSN AI Bootcamp.

Problem Statement

Predict total_sales for a given product at a given DSN Mart store, using historical product-store sales data. The competition is scored by RMSE (Root Mean Squared Error) — lower is better.

Approach
Trained multiple regression models on historical product-store sales data.
Generated several candidate submissions from different model runs/configurations.
Evaluated each submission via Kaggle's public leaderboard score.
Built a simple ensemble (row-wise average) of the two best-performing submissions to attempt a further RMSE improvement.
Results
Submission	Kaggle RMSE
dsn_submission.csv	1072.63044 (best)
dsn_submission(1).csv	1072.79393
Other candidate submissions	Did not beat the above
dsn_submission_ensemble.csv (avg of top two)	Pending submission
Repository Contents
dsn_submission_ensemble.ipynb — notebook that loads the two best submissions, averages predictions row-by-row, and writes the ensemble CSV.
dsn_submission_ensemble.csv — output of the ensemble notebook, ready for Kaggle submission.
How to Run
Place your submission CSVs (each with id and total_sales columns) in the project directory.
Open dsn_submission.ipynb
Run all cells to produce dsn_submission_ensemble.csv.
Submit the resulting file to the Kaggle competition page.
Next Steps
Submit the ensemble file and compare its RMSE against the individual models.
Experiment with weighted averaging (favoring the stronger model) instead of a straight 50/50 blend.
Explore feature engineering and additional models to push RMSE lower ahead of the DSN AI Bootcamp selection.
Context

This project is part of qualification for the DSN AI Bootcamp. Leaderboard performance is one input into selection, alongside other criteria.
