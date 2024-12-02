# Water Quality Analysis

## Overview
This project analyzes water quality based on various physical and chemical properties to predict its potability (safe or unsafe for drinking). Using Python and machine learning, the project explores key factors that affect water quality and trains a model to classify water samples as potable or unpotable.

---

## Dataset
The dataset contains the following features:
- **ph**: pH value of water.
- **Hardness**: Water hardness in mg/L.
- **Solids**: Total dissolved solids in ppm.
- **Chloramines**: Chloramine concentration in ppm.
- **Sulfate**: Sulfate concentration in mg/L.
- **Conductivity**: Electrical conductivity of water in μS/cm.
- **Organic_carbon**: Organic carbon concentration in ppm.
- **Trihalomethanes**: Concentration of trihalomethanes in μg/L.
- **Turbidity**: Measure of water clarity in NTU.
- **Potability**: Target variable indicating water safety (1 = Safe, 0 = Unsafe).

### Source
The dataset is sourced from [Kaggle](https://www.kaggle.com/) and contains essential features for evaluating water quality.

---

## Installation

### Step 1: Clone the Repository
```
git clone https://github.com/yourusername/water-quality-analysis.git
cd water-quality-analysis
```
### Step 2: Install Dependencies
Install the required Python libraries:
```
pip install -r requirements.txt
```
### Step 2: Install Dependencies
Install the required Python libraries:
```
pip install -r requirements.txt
```

---

## Project Workflow

### 1. Data Preprocessing
- Removed rows with missing values.
- Cleaned and prepared data for analysis.

### 2. Exploratory Data Analysis (EDA)
- Visualized the distribution of potable (safe) and unpotable (unsafe) water.
- Analyzed individual features like pH, Hardness, Solids, and their impact on potability.

### 3. Model Training
- Used **PyCaret** to compare various classification models.
- Selected **Random Forest Classifier** as the best-performing algorithm.

### 4. Predictions
- Evaluated the model on test data.
- Made predictions on water potability based on provided features.

---

## Usage

### Running the Project
1. Open the terminal in the project directory.
2. Run the following script to train the model and generate results:
   ```
   python water_quality_analysis.py
   ```
   
---

## Results

- The **Random Forest Classifier** was selected as the best-performing model.

### Example Results:
- **Input Features**: pH = 7.5, Hardness = 150, Solids = 20000.
- **Output**: Predicted Potability = 1 (Safe).

---

## Dependencies

- Python 3.7+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- PyCaret
- Plotly

---

## Future Improvements

- Handle imbalanced data to improve predictions for rare categories.
- Include additional features to enhance water quality classification.
- Deploy the project as an interactive web application using Streamlit.

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or improvements.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Acknowledgements

- **Dataset**: Sourced from Kaggle.
- **Inspiration**: Inspired by Aman Kharwal's article on water quality analysis.
- **Libraries and Tools**: Built using Python, Pandas, Matplotlib, and PyCaret.

---

## Repository Structure

```
water-quality-analysis/

│

├── water_quality_analysis.py   # Main Python script for the project

├── water_potability.csv         # Dataset file

├── requirements.txt             # List of required libraries

├── README.md                    # Project documentation

└── LICENSE                      # License file

```
