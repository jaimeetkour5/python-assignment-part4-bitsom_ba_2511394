# README.md: Student Performance Analysis & Prediction

## Project Overview
This project provides an end-to-end data science pipeline to analyze student performance and predict academic outcomes. Using a sample dataset of 15 students, the project covers data ingestion, exploratory data analysis (EDA), statistical visualization, and machine learning classification.

## Key Features

### 1. Data Exploration (Pandas)
- **Ingestion:** Loading raw data into a structured DataFrame.
- **Descriptive Statistics:** Analyzing means, standard deviations, and distributions of subject scores.
- **Comparative Analysis:** Calculating average subject performance specifically for students who passed versus those who failed.
- **Ranking:** Identifying top-performing students by calculating an across-the-board `overall_avg`.

### 2. Statistical Visualization
- **Matplotlib Suite:** Five custom plots including histograms for score distribution, scatter plots for study habits, and box plots for attendance trends.
- **Seaborn Suite:** Advanced statistical plots including grouped bar charts and linear regression plots to visualize the relationship between attendance and final grades.
- **Comparison:** The project demonstrates that while Matplotlib offers granular control, Seaborn simplifies complex statistical mapping (like hue-based regression lines).

### 3. Machine Learning Pipeline (Scikit-learn)
- **Preprocessing:** Features include grades (Math, Science, English, History, PE), attendance percentage, and study hours. Data is normalized using `StandardScaler` to ensure model stability.
- **Modeling:** A **Logistic Regression** classifier is trained to predict the binary `passed` target.
- **Evaluation:** The model is evaluated on a test set, with individual predictions compared against actual results.
- **Interpretability:** Feature importance is visualized via model coefficients, highlighting which factors (e.g., study hours vs. specific subjects) most heavily influence a "Pass" prediction.

## File Outputs
The notebook automatically generates and saves the following visualizations as `.png` files:
- `plot1_bar.png` to `plot5_line.png` (Matplotlib)
- `plot6_seaborn_bar.png` & `plot7_seaborn_scatter.png` (Seaborn)
- `plot8_feature_importance.png` (ML Interpretability)

## Conclusion
This analysis demonstrates the full lifecycle of a data project. Despite the small dataset, the model identifies clear trends: consistent attendance and study hours are the strongest predictors of student success. This framework can be easily scaled to larger datasets for more robust predictive modeling.