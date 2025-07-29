<<<<<<< HEAD
# DVC Bento Demonstration (In Progress)

This repository demonstrates a machine learning workflow using [DVC](https://dvc.org/) for data version control and [BentoML](https://bentoml.com/) for model serving. The project uses the Titanic dataset to train a logistic regression model to predict passenger survival.

## Project Structure

- `data_download.ipynb`: Jupyter notebook to download the Titanic dataset.
- `data/`: Contains the Titanic dataset and DVC tracking files.
- `dvc-bento-demonstration/`: Main project directory with code, model artifacts, and DVC configuration.
  - `train_model.py`: Script to train a logistic regression model on the Titanic dataset and save it using BentoML.
  - `service.py`: Example BentoML service (in progress).
  - `test_titanic_service.py`: Placeholder for service tests.
  - `scaler.pkl`, `titanic_model.pkl`: Model artifacts (may be generated during development).
  - `.dvc/`, `.gitignore`, `.dvcignore`: DVC and Git configuration files.

## Getting Started

1. **Download the Data**

   Run the notebook to download the Titanic dataset:

   ```sh
   jupyter notebook data_download.ipynb
   ```

2. **Train the Model**

   From the `dvc-bento-demonstration` directory, run:

   ```sh
   python train_model.py
   ```

   This will train a logistic regression model and save it using BentoML.

3. **Model Serving**

   The BentoML service in `service.py` is a placeholder and will be developed further.

## Requirements

- Python 3.10+
- pandas
- scikit-learn
- bentoml
- dvc

Install dependencies with:

```sh
pip install -r requirements.txt
```

*(Create a `requirements.txt` if needed.)*

## Notes

- This project is **in progress**. The BentoML service and testing are not yet complete.
- Data files are tracked with DVC; use `dvc pull` to retrieve data if needed.

## License

This project is for demonstration and educational purposes.
