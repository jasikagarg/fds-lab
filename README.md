# fds-lab
This README provides a comprehensive evaluation of two iterations of the Mental Health Dataset (Version 1 and Version 2) regarding their capabilities across the four levels of data analytics: Descriptive, Diagnostic, Predictive, and Prescriptive.

1. Dataset Version 1: Global General Population Dataset (mental_health_dataset.csv)

Dataset Profile

Scope: 1,000 observations covering working professionals and students globally.

Key Features: Age, Gender, Occupation, Country, Mental Health Condition, Severity, Stress Level, Sleep Hours, Work Hours, Physical Activity Hours, Consultation History.

Analytics Capability Evaluation

🟢 Descriptive Analytics → Strong

Capability: High

Explanation: The dataset excels at providing baseline summary statistics and demographic distributions (e.g., average sleep hours per country, distribution of stress levels across occupations, proportion of individuals with diagnosed mental health conditions).

🟢 Diagnostic Analytics → Moderate to Strong

Capability: Moderate to High

Explanation: Enables comparative and correlation analyses to explore why certain trends exist. Correlations between work hours, sleep hours, physical activity, and stress/severity levels can be established using hypothesis testing (e.g., Chi-Square, ANOVA).

🟡 Predictive Analytics → Partial

Capability: Moderate

Explanation: Suitable for supervised classification algorithms (e.g., Logistic Regression, Random Forest, XGBoost) to predict Mental_Health_Condition or Stress_Level. However, prediction accuracy is limited because the data is cross-sectional (single point in time) rather than longitudinal (tracking individuals over time).

🔴 Prescriptive Analytics → Weak / Missing

Capability: Low / Limited

Explanation: The dataset lacks outcome metrics from specific interventions, cost constraints, or decision-optimization parameters. While general domain rules can be inferred (e.g., "reduce work hours"), the dataset does not directly support optimization or decision-tree models for prescriptive strategies.

2. Dataset Version 2: Student Lifestyle & Mental Well-being Dataset (Mental_Health_Dataset_Version_2.csv)

Dataset Profile

Scope: Primary survey data focused on university students (undergraduate and postgraduate).

Key Features: Academic & Entertainment Screen Time, Likert-scale psychological metrics (Anxiety, Racing Thoughts, Concentration, Motivation, Irritability), Physical Energy, Water Intake, Meal Regularity, Dietary Habits, Digestive Discomfort, and Qualitative Open-Ended Factors.

Analytics Capability Evaluation

🟢 Descriptive Analytics → Strong

Capability: High

Explanation: Provides rich, multi-dimensional profiles of student populations. It captures academic vs. entertainment screen time, sleeping patterns, hydration, dietary intake, and multi-item psychological symptom scores.

🟢 Diagnostic Analytics → Strong

Capability: High

Explanation: Exceptional root-cause investigation capability. The dataset combines quantitative metrics with qualitative text entries describing emotional stressors (e.g., exams, doomscrolling, relationship stress, night shifts). Natural Language Processing (NLP) / Sentiment Analysis on qualitative entries further enriches diagnostic insights.

🟡 Predictive Analytics → Partial

Capability: Moderate

Explanation: Provides a richer feature set for predicting high stress or mental exhaustion compared to Version 1 (using screen time breakdown, sitting duration, meal habits, etc.). However, like Version 1, it remains snapshot/cross-sectional survey data, preventing dynamic time-series forecasting.

🟡 Prescriptive Analytics → Partial / Emerging

Capability: Moderate-Low

Explanation: Closer to actionable prescription than Version 1 because it measures highly controllable daily habits (water intake, sitting breaks, screen time limits, meal timing). Targeted action recommendations (e.g., "Limit non-academic screen time to under 3 hours to reduce sleep delay") can be derived, though explicit intervention testing data is absent.

3. Comparison Summary Matrix

Analytics Technique

Version 1 (mental_health_dataset.csv)

Version 2 (Mental_Health_Dataset_Version_2.csv)

Descriptive (What happened?)

🟢 Strong: Demographic & work profile summaries

🟢 Strong: Detailed student lifestyle & multi-symptom breakdown

Diagnostic (Why did it happen?)

🟢 Moderate-Strong: Correlation between work/sleep and stress

🟢 Strong: Combined quantitative scales & qualitative stressor descriptions

Predictive (What will happen?)

🟡 Partial: Basic classification of condition/stress level

🟡 Partial: Higher feature resolution for predicting fatigue/anxiety

Prescriptive (What should we do?)

🔴 Weak: Lacks actionable daily behavioral variables

🟡 Partial: Measures actionable daily habits (screen time, diet, break frequency)

4. Recommendations for Next Dataset Iteration (Moving to Full Predictive & Prescriptive)

To elevate future datasets to Full Predictive and Full Prescriptive status, consider adding:

Longitudinal Time-Series Tracking: Capture daily or weekly logs over 4–8 weeks for individual students.

Intervention / AB Testing Metrics: Track whether students who implemented specific recommendations (e.g., setting screen time locks, taking 5-minute break intervals) showed measured stress reduction.

Constraint & Resource Features: Include student available study hours, workload constraints, or access to counseling support.
