# 📊 Product A/B Test Analysis

## 📌 Description
This project analyzes the impact of a typography change in a food company’s
mobile application using an A/A/B experiment to evaluate whether the change
produces a statistically significant effect on user behavior.

The analysis focuses on user behavior across an event funnel, first validating
the equivalence of the control groups (A/A) and then evaluating the effect of
the typography change (A/B).

## 🧠 Objective
- Evaluate the impact of a typography change on user behavior
- Validate user group assignment through an A/A test
- Analyze the application event funnel
- Apply statistical tests with multiple testing correction
- Draw data-driven business conclusions

## 📂 Project Structure
- `datasets/` → Experiment dataset
- `notebooks/` → A/A/B analysis notebook
- `README.md` → Project description in Spanish
- `README_EN.md` → Project description in English

## 🔬 Methodology
- Data cleaning and preprocessing
- Exploratory analysis of user behavior
- Event funnel analysis
- A/A test to validate control group equivalence
- A/B test to measure typography impact
- Significance level adjustment for multiple testing

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- SciPy
- Matplotlib / Seaborn
- Jupyter Notebook

## 📈 Results

The main objective of the experiment was to evaluate whether a change in the
application’s typography had a significant impact on user behavior. An A/A/B
experiment was conducted, including two control groups (246 and 247) and one
test group (248) exposed to the new design.

The analysis leads to the following key conclusions:

- **Experiment validity:**  
  The comparison between the two control groups showed no statistically
  significant differences across any of the analyzed events, confirming that
  the randomization was successful and the experiment was correctly designed.

- **Redesign impact:**  
  When comparing the group exposed to the new typography (248) against the
  control groups, no statistically significant differences were found in the
  key events of the conversion funnel (main screen, offers, cart, payment,
  and tutorial).

- **Statistical robustness:**  
  A total of 15 hypothesis tests were performed. After applying the Bonferroni
  correction to control for multiple testing, all conclusions remained
  consistent. The lowest observed p-value was still above the adjusted
  threshold (0.0033), indicating no detectable effect attributable to the
  redesign.

In conclusion, since the typography change does not negatively affect user
behavior, its full implementation is recommended. Additionally, the experiment
validates the robustness of the product’s experimentation framework and
provides a solid foundation for future, more complex A/B tests.
