Titanic Dataset - Exploratory Data Analysis (EDA)
📄 Project Overview

This project performs Exploratory Data Analysis (EDA) on the Titanic dataset (Titanic-Dataset.csv) to understand the data, uncover patterns, trends, and anomalies, and make basic feature-level inferences. The goal is to gain insights into factors affecting passenger survival using statistics and visualizations.

🛠 Tools and Libraries Used

Python 3.x

Pandas – for data loading, manipulation, and summary statistics

Matplotlib – for plotting histograms, boxplots, and bar charts

Seaborn – for enhanced visualization (heatmaps, pairplots, distribution plots)

🔹 Steps Performed
1. Generate Summary Statistics

Computed mean, median, standard deviation, min, max, and quartiles for numeric features.

Examined categorical feature distributions using counts and unique values.

Insights:

Average passenger age ≈ 29.7 years

Average fare ≈ 32.2

38% of passengers survived

2. Create Histograms and Boxplots

Plotted histograms to understand feature distributions.

Used boxplots to detect outliers.

Observations:

Fare is highly skewed with extreme outliers

Age shows a roughly normal distribution with missing values

Most passengers traveled alone (SibSp and Parch mostly 0)

3. Pairplot and Correlation Matrix

Correlation heatmap to identify relationships between numeric features.

Pairplot to visualize scatterplots and distributions.

Key findings:

Negative correlation between Fare and Pclass (higher class → higher fare)

Weak correlation of Age and Fare with survival

4. Identify Patterns, Trends, or Anomalies

Sex: Females had higher survival than males

Pclass: 1st class passengers survived more than 3rd class

Age: Children had better survival rates; elderly less likely

Fare: Highly skewed; some extreme outliers (wealthy passengers)

SibSp/Parch: Most passengers traveled alone; few large families (outliers)

5. Basic Feature-Level Inferences from Visuals

Sex is a strong predictor of survival

Passenger class influences survival chances

Age affects survival, especially children and young adults

Fare indicates socioeconomic advantage → better survival odds

Family size can influence travel and survival patterns

📊 Visualizations Created

Histograms & Boxplots for numeric features (Age, Fare, SibSp, Parch)

Barplots for categorical vs target (Sex, Pclass)

Correlation heatmap for numeric feature relationships

Pairplot for scatterplots and distributions
