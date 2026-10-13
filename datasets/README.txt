Employee Attrition Insight — Synthetic Practice Dataset

These five CSV files are synthetic and generated for learning/assessment practice.
They are NOT real company or employee data and must not be presented as actual company findings.

Files:
- employees.csv: employee profile, department, role, tenure, grade, age
- attendance.csv: absences, monthly overtime, leave days
- compensation.csv: salary band, increment percentage, benefits score
- engagement.csv: engagement score and survey participation
- movement.csv: promotion/transfer history and exit status

Join key: employee_id

Intentional data quality issues:
- employees.csv contains 8 duplicate employee records and inconsistent role capitalization/spacing.
- engagement.csv contains missing engagement scores.
- attendance.csv contains several extreme overtime values.
- movement.csv contains unknown/missing promotion-history values.

Suggested workflow:
1. Inspect shapes, dtypes, missing values and duplicate IDs.
2. Clean duplicates and standardize role names.
3. Investigate outlier overtime values before treating them.
4. Merge on employee_id after checking key uniqueness.
5. Predict exit_status using only information available before the exit decision.
6. Report metrics and findings from your own model run.
