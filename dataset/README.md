# Dataset

The `dataset/raw/attrition_data.csv` file contains the employee records used to train and validate the attrition model in this repository.

Important notes:

- The production model bundled in `models/` was trained on this CSV specifically. For accurate predictions and reproducible results, upload this exact CSV to the Streamlit app before using **Data Explorer**, **Batch Prediction**, or **Individual Prediction**.
- Required features for predictions: `MonthlyIncome`, `JobSatisfaction`, `YearsAtCompany`, `OverTime`, `WorkLifeBalance`, `DistanceFromHome`.
- Keep the CSV in `dataset/raw/` if you plan to retrain or re-run the notebook.

If you wish to use a different dataset, ensure it contains the required features and the same encoding conventions (e.g., `OverTime` recorded as `Yes`/`No` or `1`/`0`).
