# Forecasting Project

This repository delivers a complete solution for analyzing and forecasting weekly SKU-level demand using Python. It features:
- In-depth exploratory data analysis (EDA) to uncover trends and patterns
- Advanced time series forecasting with ARIMA, LSTM, and Prophet models
- Interactive visualizations for actionable business insights


## Project Structure

```
requirements.txt
README.md

data/
    ForecastDataset_from_2016_To_2024_for_all_SKUs.csv
    ForecastDataset_from_2016_to_2025_for_SKUs_started_with_90.csv
    ForecastDataset.csv
    SKUForecastDataSet.xlsx
    testing_data.csv
    training_data.csv
eda/
    EDA.ipynb
model_results/
    actual_vs_forecast.csv
    actual_vs_predicted_forecast_results.csv
    enhanced_prophet_forecast_results.csv
    lstm_forecast_results_90AD350AD01.csv
    optimized_prophet_forecast.csv
    SKU_Forecasts.xlsx
models/
    arima_model.ipynb
    lstm_model.ipynb
    prophet_model.ipynb
research_notebooks/
    2016_To_2024_data_for_all_skus.ipynb
    data.ipynb
    forecasting.ipynb
    prophet.ipynb
    Top_5_skus_forecasting_started_with_90.ipynb
```


## Requirements

- Python 3.13.5 (recommended) or Python 3.8+
- pip (Python package manager)

### Main Python Packages
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- statsmodels
- scikit-learn
- openpyxl
- tensorflow (for LSTM)
- prophet (for Prophet model)


All required packages are listed in `requirements.txt`.



## Installation Steps

1. **Clone the Repository**
   ```powershell
   git clone https://github.com/Agivant-Technologies-India-Pvt-Ltd/forecasting.git
   cd forecasting
   ```

2. **Set Up a Virtual Environment (Recommended)**
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

3. **Install Requirements**
   ```powershell
   pip install --upgrade pip
   pip install -r requirements.txt
   ```

   If you encounter issues with `prophet`, install it separately:
   ```powershell
   pip install prophet
   ```

4. **(Optional) Install Jupyter Notebook**
   ```powershell
   pip install notebook
   ```

5. **Launch Jupyter Notebook**
   ```powershell
   jupyter notebook
   ```
   Open and run notebooks in the `eda/`, `models/`, or `research_notebooks/` folders.

## Running in Visual Studio Code (VS Code)

1. **Open the Project in VS Code**
   - Launch VS Code.
   - Go to `File` > `Open Folder...` and select the `datasets` folder inside the root `forecasting` folder (i.e., open `forecasting/datasets`).

2. **Select the Python Interpreter**
   - Press `Ctrl+Shift+P` (or `F1`) to open the Command Palette.
   - Type `Python: Select Interpreter` and choose the `.venv` environment (it should show as `.venv` or similar).

3. **Install the Python Extension (if not already installed)**
   - Go to the Extensions view (`Ctrl+Shift+X`).
   - Search for `Python` and install the official Microsoft Python extension.

4. **(Optional) Install Jupyter Extension**
   - In the Extensions view, search for `Jupyter` and install it for notebook support.

5. **Activate the Virtual Environment in the VS Code Terminal**
   - Open a new terminal in VS Code (`Ctrl+`` or `Terminal` > `New Terminal`).
   - If not already activated, run:
     ```powershell
     .\.venv\Scripts\activate
     ```

6. **Install Requirements (if not already done)**
   - In the terminal, run:
     ```powershell
     pip install --upgrade pip
     pip install -r requirements.txt
     ```

7. **Open and Run Notebooks**
   - Open any `.ipynb` file (e.g., `eda/EDA.ipynb`).
   - Click `Run All` or run cells individually.

8. **Run Python Scripts (if any)**
   - Open the script file and press `F5` or right-click and select `Run Python File in Terminal`.

You are now ready to explore, analyze, and forecast using the provided notebooks and scripts in VS Code!

 
## Usage

- **Data**: Place your data files in the `data/` directory.
- **EDA**: Start with `eda/EDA.ipynb` for exploratory data analysis.
- **Modeling**: Use notebooks in `models/` for ARIMA, LSTM, and Prophet forecasting.
- **Results**: Find output and results in the `model_results/` directory.


## Notes
- For LSTM, ensure TensorFlow is installed and your system supports it.
- For Prophet, installation may require a C++ compiler (see Prophet documentation if you have issues).
- All code is compatible with Python 3.13.5 and Python 3.8+.

## Troubleshooting
- If you face issues with package installation, try upgrading pip or installing packages one by one.
- For Windows, run PowerShell as Administrator if you encounter permission errors.


