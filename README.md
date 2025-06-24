# Multivariate-Statistical-Analysis-for-The-Students-Habits-and-Academic-Performance-Dataset
This project explores how students’ lifestyle habits influence their academic performance using multivariate statistical techniques. The analysis is based on a dataset of 1,000 students with over 15 variables, including study hours, sleep patterns, social media usage, exercise frequency, mental health ratings, and exam scores.

By applying Principal Component Analysis (PCA), Factor Analysis (FA), Linear Discriminant Analysis (LDA), and Canonical Correlation Analysis (CCA) in R, the project aims to:

-  Identify key patterns and latent factors in student habits and performance

-  Classify students into performance groups based on their lifestyle characteristics

-  Explore relationships between academic outcomes and well-being-related factors

The findings highlight the importance of study habits, wellness practices, and reduced digital distractions in achieving academic success.

📌 Tools & Technologies: R (MASS, caret, heplots, car, CCA, CCP, and other packages)

Feel free to explore the code, data insights, and visualizations to gain a deeper understanding of the multivariate relationships uncovered in this analysis.

📊 ##**Dataset Description**

The dataset used in this project, student_habits_performance.csv, contains records of 1,000 students, capturing their academic habits, lifestyle factors, and performance outcomes. The data was sourced from Kaggle.

It includes 15 variables categorized as follows:

**1. Continuous Variables (9):**

- age — age of the student

- study_hours_per_day — average daily study hours

- social_media_hours — average daily time spent on social media

- netflix_hours — average daily time spent watching Netflix

- attendance_percentage — class attendance rate

- sleep_hours — average daily sleep hours

- exercise_frequency — weekly frequency of physical exercise

- mental_health_rating — self-reported mental health score

- exam_score — final exam score

**2. Categorical Variables (6):**

- gender — male/female

- part_time_job — employment status

- diet_quality — self-rated diet quality

- parental_education_level — highest parental education

- internet_quality — quality of internet access

- extracurricular_participation — participation in extracurricular activities

**3. Identifier:**

- student_id — unique ID for each student

👉 The dataset is clean, with no missing values, making it suitable for multivariate statistical analysis.

🔬##** Statistical Methods Applied**
Several advanced multivariate techniques were applied using R to explore patterns, reduce dimensionality, classify groups, and analyze relationships between student lifestyle habits and academic performance:

1️⃣ **Principal Component Analysis (PCA)**
- PCA was used to reduce the dimensionality of the dataset while retaining as much variance as possible.

- The first six principal components explained approximately 78.7% of the total variance.

- PCA helped identify key combinations of variables that capture most of the information in the dataset, simplifying further analysis.

2️⃣ **Factor Analysis (FA)**
- FA aimed to uncover latent factors that explain the relationships among observed variables.

- Analysis focused on academic effort as the main driver of exam scores, with lifestyle factors playing secondary roles.

- A two-factor solution was selected to balance model fit and interpretability, supported by parallel analysis and eigenvalue criteria.

3️⃣ **Linear Discriminant Analysis (LDA)**
- LDA was applied to classify students into high and low performance groups (based on the median exam score).

- Key discriminators included study_hours_per_day, mental_health_rating, attendance_percentage, and digital media usage.

- The model achieved a high classification accuracy of over 90%, validated through cross-validation.

4️⃣ **Canonical Correlation Analysis (CCA)**
- CCA explored the multivariate relationships between two sets of variables:

-    Lifestyle set: social_media_hours, netflix_hours, sleep_hours, exercise_frequency, mental_health_rating

-    Academic set: study_hours_per_day, attendance_percentage, exam_score

The first canonical correlation (0.8355) indicated a strong link between a healthier lifestyle (better mental health, more exercise and sleep, less digital distraction) and better academic outcomes.

⚙ **Tools and Software**
R (v4.3.0)

Key packages: MASS, caret, heplots, car, CCA, CCP, and others

👉 This analysis provides valuable insights into how student habits influence academic success and offers a foundation for further predictive modeling or clustering.
