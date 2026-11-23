Features:
person_id |
age |
gender |
nationality |
first_generation |
disability_status | 
family_income_level | 
scholarship_holder |
tuition_up_to_date |  
part_time_job | 
weekly_work_hours |
course_type | 
study_mode | 
semester | 
international_student |
admission_grade | 
previous_qualification_grade | 
units_enrolled |
units_passed | 
units_failed | 
gpa_semester_1 | 
gpa_semester_2 |
attendance_rate | 
assignments_submitted_rate |
library_visits_per_month | 
lms_logins_per_week |
extracurricular_activities | 
missed_deadlines | 
stress_level |
mental_health_support | 
satisfaction_score | 
commute_time_mins |
sleep_hours | 
--------------------------------------------------------------------
Target: dropout
--------------------------------------------------------------------
Training set = 70%
Test set = 30%

No missing value
Non-numeric values: gender - nationality - family_income_level - course_type - study_mode   

Based on Scikit-learn's cheatsheet on choosing the model: SGD Classifier

Baseline model with 5-fold Searchcv: SGD Classifier

Stochastic Gradient Descent is sensitive to feature scaling, so it is highly recommended to scale your data. This can be easily done using StandardScaler.

Mean baseline CV validation accuracy: 83.15%

Baseline test accuracy: 83.84%

              precision    recall  f1-score   support

           0       0.87      0.90      0.88     20399
           1       0.77      0.70      0.74      9601

    accuracy                           0.84     30000
    
   macro avg:       0.82   |   0.80   |   0.81  |   30000
   
weighted avg:       0.84   |   0.84   |   0.84  |   30000


