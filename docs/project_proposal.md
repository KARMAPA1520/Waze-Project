# Project Proposal — Waze User Churn

## 1. Business Problem
Waze leadership needs to understand and anticipate monthly user churn.
Users who uninstall or stop opening the app represent lost engagement,
reduced map data quality, and reduced advertising reach. Currently there
is no systematic way to identify at-risk users before they leave.

## 2. Project Goal
Build a model that predicts whether a user will churn, and identify the
behavioral factors most associated with churn, so the product team can
target retention efforts.

## 3. Stakeholders
| Role | Interest in this project |
|:-----|:-------------------------|
| Data Analysis Team | Owns the analysis and modeling |
| Product Managers | Use insights to prioritize retention features |
| Marketing / Growth | Target at-risk segments with campaigns |
| Leadership | Business impact and resourcing decisions |

## 4. Initial Hypotheses
- Users with fewer active days per month are more likely to churn.
- Users churn more in their first weeks after onboarding, before the app
  becomes habitual.
- Device type (iPhone vs. Android) is *not* associated with churn.

*(These are stated up front so the Analyze phase tests them rather than
retrofitting conclusions to whatever the data shows.)*

## 5. Data Overview
- **Source:** Waze dataset, Google Advanced Data Analytics Certificate
- **Rows / columns:** _fill in after Milestone 3_
- **Target variable:** `label` (retained / churned)
- **Known issue:** the `label` column contains missing values that must be
  assessed before modeling

## 6. Success Criteria
- A model that predicts churn better than a majority-class baseline
- A ranked list of features associated with churn
- Findings communicated in a format non-technical stakeholders can act on

## 7. Scope and Limitations
- The dataset covers one month; seasonal and long-term patterns cannot
  be assessed.
- No qualitative data (surveys, support tickets), so the analysis can show
  *what* correlates with churn, not *why* users decide to leave.

## 8. Ethical Considerations
Predicting churn drives targeted interventions. False positives mean users
receive unwanted outreach; false negatives mean at-risk users are missed.
Since the cost of a missed churner is higher than a wasted notification,
recall should be weighted above precision.