# Group Member 2: Data Strategy & Preprocessing

---

## 🔹 Part 1: Short Answer Questions

### Q2: Data Collection & Preprocessing

**1. Identify 2 data sources for your problem:**

- **Electronic Health Records (EHRs)** – contain patient visit history, diagnoses, discharge notes, medication records, and lab results.
- **Demographic data** – includes age, gender, location, and income level (may be collected via patient intake forms or national health databases).

---

**2. One potential bias in the data:**

- **Underrepresentation Bias** – The dataset may have fewer samples from rural or low-income populations, making predictions less accurate for these groups.

---

**3. Preprocessing steps:**

- **Handling missing values:** Fill missing lab results with median values or flag them with binary indicators.
- **Normalization:** Scale continuous features like age or lab values using Min-Max scaling.
- **Encoding categorical features:** Convert diagnosis or discharge status into numerical format using one-hot encoding.

---

## 🔹 Part 2: Case Study Application – Data Strategy

### 1. Data Sources:

- **Hospital Electronic Health Records (EHRs):**
  - Admission & discharge notes
  - Previous readmissions
  - Diagnosis codes (ICD-10)
  - Prescriptions

- **Demographics & Socioeconomic Info:**
  - Age, gender, ethnicity
  - Zip code, income brackets
  - Insurance coverage

---

### 2. Ethical Concerns:

- **Patient Privacy:** Sensitive health data must be protected with encryption and data anonymization to comply with healthcare privacy laws like HIPAA.
- **Algorithmic Bias:** If training data is skewed toward a certain population (e.g., urban patients), the model may be less effective for underrepresented groups.

---

### 3. Preprocessing Pipeline:

1. **Data Cleaning**
   - Drop rows with excessive missing values
   - Replace missing numerical values with median or mean

2. **Feature Engineering**
   - Create features like `Days Since Last Visit`, `Total Hospital Stays in Past Year`, etc.

3. **Encoding & Scaling**
   - Apply one-hot encoding to categorical columns (e.g., Diagnosis Code)
   - Normalize age, blood pressure, and other numerical features

4. **Train-Test Split**
   - Reserve 70% of data for training, 30% for testing

5. **Class Balancing (if needed)**
   - Use SMOTE (Synthetic Minority Oversampling) if readmitted patients are underrepresented



