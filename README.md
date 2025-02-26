# Credit Risk Modeling with Machine Learning

## Project Overview
This project aims to build a machine learning model to predict the credit risk level of a customer applying for a credit card. The output is a categorical variable with four risk levels:

- **P1**: Very good customer, unlikely to default.
- **P2**: Good customer, slightly higher risk than P1.
- **P3**: Moderate risk customer.
- **P4**: High-risk customer, more likely to commit fraud.

We used Python and Jupyter Notebook to prepare the data, perform statistical analysis, and build several machine learning models, ultimately achieving the best accuracy with the XGBoost algorithm.

---

## Datasets
We combined two datasets using an **inner join**:

### Case Study 1: Internal Data (Trade Line Details)
- **Total_TL**: Total trade lines/accounts in Bureau
- **Tot_Closed_TL**: Total closed trade lines/accounts
- **Tot_Active_TL**: Total active accounts
- **Tot_Missed_Pmnt**: Total missed payments
- **CC_TL**: Count of credit card accounts
- **Age_Oldest_TL**: Age of oldest opened account
- **Age_Newest_TL**: Age of newest opened account
- *(And many more features related to trade lines and account history)*

### Case Study 2: External Data (CIBIL and Delinquency Details)
- **time_since_recent_payment**: Time since recent payment
- **num_times_delinquent**: Number of times delinquent
- **num_std**: Number of standard payments
- **num_sub**: Number of substandard payments
- **CC_utilization**: Credit card utilization
- **PL_utilization**: Personal loan utilization
- **Credit_Score**: Applicant’s credit score
- **Approved_Flag**: Priority level (target variable)
- *(And many more features related to delinquency, inquiries, and loan usage)*

---

## Data Preprocessing
1. **Data Cleaning**:
   - Removed null values.
   - Dropped columns with excessive missing values.

2. **Data Merging**:
   - Merged datasets using an inner join on customer ID.

3. **Encoding**:
   - Categorical encoding for nominal and ordinal features.

4. **Feature Selection**:
   - **Chi-Square Test** for categorical variables.
   - **ANOVA** for numerical variables.
   - **Sequential Variance Inflation Factor (VIF)** to detect and remove multicollinearity.

---

## Machine Learning Models
We built and evaluated multiple models:

- **Decision Tree**
- **Random Forest**
- **XGBoost (Best Performance)**

**Hyperparameter Tuning:** Performed using **GridSearchCV** to optimize model performance.

---

## Results
The **XGBoost model** achieved the best accuracy, making it the final chosen model for deployment.

---

## Project Structure
```
├── data/
├── notebooks/
├── models/
├── results/
├── README.md
```

---

## How to Run the Project
1. **Clone the repository:**
```bash
git clone https://github.com/yourusername/credit-risk-modeling.git
```

2. **Navigate to the project folder:**
```bash
cd credit-risk-modeling
```

3. **Launch Jupyter Notebook:**
```bash
jupyter notebook
```

4. **Run the notebook cells to execute the entire workflow.**

---

## Conclusion
This project successfully built a credit risk prediction model using statistical techniques and machine learning algorithms. It provides valuable insights for financial institutions to assess customer risk levels and make informed credit card approval decisions.

Feel free to contribute or reach out if you have any suggestions!

---

## Author
**Your Name**  
📧 sachinghogare1762@gmai.com  
🔗 [LinkedIn][(www.linkedin.com/in/sachin-ghogare-325427208)](https://www.linkedin.com/in/sachin-ghogare-325427208/)

---



