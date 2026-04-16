# Titanic Machine Learning Project

## Overview
This project analyzes the Titanic dataset to predict passenger survival using machine learning classification models. The analysis includes comprehensive exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and interactive visualizations.

## Goal
Predict passenger survival on the Titanic disaster using classification models, achieving high accuracy and providing insights into the factors that influenced survival rates.

## Aim
- Build and compare multiple machine learning models (Logistic Regression, Random Forest, Gradient Boosting, Voting Ensemble)
- Perform thorough exploratory data analysis to understand data patterns and correlations
- Create interactive visualizations for data exploration and presentation
- Implement advanced feature engineering techniques
- Provide deployment-ready models with comprehensive documentation

## Steps

### 1. Data Preprocessing (`Titanic_Preprocessing.ipynb`)
- Load and explore the Titanic dataset
- Handle missing values (Age, Embarked, Fare)
- Encode categorical variables (Sex, Embarked)
- Normalize numerical features
- Split data into training and testing sets

### 2. Exploratory Data Analysis (`Titanic_Analysis.ipynb`)
- Analyze survival statistics by demographics
- Examine feature correlations and distributions
- Train baseline models (Logistic Regression, Random Forest, Gradient Boosting)
- Evaluate model performance with accuracy, precision, recall, F1-score, and ROC-AUC
- Generate confusion matrices and ROC curves
- Analyze feature importance

### 3. Interactive Dashboard (`Titanic_Dashboard.ipynb`)
- Create 9 interactive Plotly visualizations
- Export visualizations as HTML files for web viewing
- Analyze survival patterns by gender, class, age, fare, and other factors

### 4. Advanced Modeling (`Titanic_Advanced_Modeling.ipynb`)
- Implement feature engineering (Title extraction, Family Size, Fare per person, Age groups)
- Perform feature selection using SelectKBest
- Conduct hyperparameter tuning with GridSearchCV
- Build ensemble models (Voting Classifier)
- Perform cross-validation and final evaluation

### 5. Summary & Deployment (`Titanic_Summary_and_Deployment.ipynb`)
- Compile project insights and key findings
- Provide deployment guide for production use
- Include business recommendations

## Using the Dashboard

The interactive dashboard provides visual insights into the Titanic dataset:

1. **Open `Titanic_Dashboard.ipynb`** in Jupyter Notebook or VS Code
2. **Run all cells** to generate the visualizations
3. **View HTML exports** in your browser:
   - `01_survival_by_gender.html` - Gender-based survival analysis
   - `02_survival_by_class.html` - Passenger class survival rates
   - `03_age_distribution.html` - Age distribution with survival overlay
   - `04_fare_distribution.html` - Fare analysis by class and survival
   - `05_correlation_heatmap.html` - Survival correlations
   - `06_family_size_impact.html` - Family size effects on survival
   - `07_age_vs_fare_scatter.html` - Age and fare relationships
   - `08_embarkation_analysis.html` - Port of embarkation analysis
   - `09_survival_overview.html` - Overall survival statistics

4. **Interact with plots**: Hover over data points, zoom, and filter to explore patterns

## Key Findings

### Survival Statistics
- **Overall Survival Rate**: 38.4%
- **Female Survival Rate**: 74.2%
- **Male Survival Rate**: 18.9%
- **First Class Survival**: 63.0%
- **Third Class Survival**: 24.2%

### Critical Factors
1. **Gender**: Most important predictor (28.5% feature importance)
2. **Passenger Class**: Strong socioeconomic influence (19.2%)
3. **Fare Amount**: Correlates with cabin location (16.3%)
4. **Age**: Younger passengers had better survival (12.6%)

### Model Performance
- **Best Model**: Voting Ensemble (ROC-AUC: 0.9156, Accuracy: 84.92%)
- **Runner-up**: Random Forest (ROC-AUC: 0.9156, Accuracy: 84.92%)
- **Baseline**: Logistic Regression (ROC-AUC: 0.8796, Accuracy: 82.15%)

### Insights
- "Women and children first" policy was enforced
- Social class strongly influenced lifeboat access
- Large families had lower survival rates due to coordination challenges
- Higher fares indicated better cabin locations and survival chances

## Files

- `train.csv` - Training dataset (891 passengers)
- `test.csv` - Test dataset (418 passengers)
- `gender_submission.csv` - Sample submission format
- `Titanic_Preprocessing.ipynb` - Data preprocessing pipeline
- `Titanic_Analysis.ipynb` - EDA and baseline modeling
- `Titanic_Dashboard.ipynb` - Interactive visualizations
- `Titanic_Advanced_Modeling.ipynb` - Advanced feature engineering and modeling
- `Titanic_Summary_and_Deployment.ipynb` - Project summary and deployment guide
- `Titanic_Preprocessing.pdf` - PDF export of preprocessing notebook

## Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Seyipeters/titanic-machine-learning.git
   cd titanic-machine-learning
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn plotly nbformat reportlab
   ```

3. **Run the notebooks** in order:
   - Start with `Titanic_Preprocessing.ipynb`
   - Continue with analysis notebooks
   - View dashboard HTML files in a web browser

## Requirements
- Python 3.9+
- Jupyter Notebook or VS Code
- Required packages: pandas, numpy, scikit-learn, matplotlib, seaborn, plotly

## Repository
[GitHub Repository](https://github.com/Seyipeters/titanic-machine-learning)

## License
This project is for educational purposes.
