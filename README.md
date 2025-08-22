
# 🩺 Medical Data Visualizer

This project visualizes and analyzes medical examination data using **matplotlib**, **seaborn**, and **pandas**.  
The dataset contains patient information such as body measurements, blood test results, and lifestyle choices.  
We explore the relationships between **cardiovascular disease, body measurements, blood markers, and lifestyle choices**.

---

## 📊 Dataset Description
The dataset `medical_examination.csv` contains rows representing patients and columns describing medical features.

| Feature                        | Type                  | Values |
|--------------------------------|-----------------------|--------|
| age                            | Objective             | int (days) |
| height                         | Objective             | int (cm) |
| weight                         | Objective             | float (kg) |
| gender                         | Objective             | categorical |
| ap_hi (Systolic BP)            | Examination           | int |
| ap_lo (Diastolic BP)           | Examination           | int |
| cholesterol                    | Examination           | 1: normal, 2: above normal, 3: well above normal |
| gluc                           | Examination           | 1: normal, 2: above normal, 3: well above normal |
| smoke                          | Subjective            | binary |
| alco                           | Subjective            | binary |
| active                         | Subjective            | binary |
| cardio (target)                | Target Variable       | binary |

---

## ⚙️ Project Tasks
1. **Data Import**: Load dataset into a DataFrame.  
2. **Overweight Column**: Add `overweight` column using BMI (BMI > 25 → 1, else 0).  
3. **Normalize Data**: Convert cholesterol and glucose values so `0 = good`, `1 = bad`.  
4. **Categorical Plot**: Show counts of categorical features (`cholesterol, gluc, smoke, alco, active, overweight`) split by `cardio`.  
5. **Heatmap**: Generate correlation heatmap after cleaning incorrect/invalid data.  

---

## 📂 Files
- `medical_data_visualizer.py` → Core functions for plotting
- `main.py` → Runs and saves the figures
- `test_module.py` → Unit tests
- `medical_examination.csv` → Dataset

---

## ▶️ Running the Project
```bash
# Clone repository
git clone https://github.com/YOUR_USERNAME/medical-data-visualizer.git
cd medical-data-visualizer

# Install dependencies
pip install -r requirements.txt

# Run analysis
python main.py
```

---

## 🛠️ Dependencies
```
matplotlib
seaborn
pandas
pytest
```

---

## 📊 Example Outputs
- **Categorical Plot** → Distribution of health indicators by cardiovascular disease.  
- **Heatmap** → Correlation matrix of medical features.  

---

## ✅ Testing
Run unit tests with:
```bash
pytest test_module.py
```
