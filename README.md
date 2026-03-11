# A/B Testing Analysis for Website Conversion Optimization

## Project Overview

This project demonstrates how companies test new product changes using **A/B testing**.

A/B testing is a statistical experiment where users are divided into two groups:

- **Control Group** – users see the current version
- **Treatment Group** – users see the new version

The goal is to check if the **new version improves user behavior**.

In this project, we simulate a website experiment and analyze whether a **new website design increases the conversion rate**.

---

# Why This Project Was Made

Companies often change product features such as:

- website design
- button color
- recommendation algorithms
- pricing strategies

If changes are released without testing, they may **harm product performance**.

A/B testing helps companies:

- test new ideas safely  
- measure the impact of product changes  
- make **data-driven decisions**

This project was created to demonstrate how **data scientists analyze experiments and determine if a change should be launched**.

---

# Who Benefits From This Project

This type of analysis is useful for:

### Product Teams
They can understand if a new feature improves user engagement.

### Data Scientists
They use statistical tests to determine if experiment results are reliable.

### Product Managers
They use experiment results to decide whether a feature should be launched.

### Companies
They reduce risk by testing ideas on small groups before releasing them to all users.

Industries that commonly use A/B testing:

- Technology companies  
- E-commerce platforms  
- Social media platforms  
- Online marketing teams  

---

# Experiment Scenario

We simulate a website experiment where a company wants to test a **new website design**.

Two groups of users are created:

| Group | Description |
|------|-------------|
| Control | Users see the current website |
| Treatment | Users see the new website design |

The main metric used is **conversion rate**.

Conversion Rate:

Conversion Rate = conversions / total users

Example:

If 100 users visit the website and 8 purchase a product:

Conversion Rate = 8%


---

# Project Workflow

### 1. Power Analysis
We estimate how many users are required for the experiment.

This ensures the experiment has enough data to detect real improvements.

---

### 2. Data Simulation

A dataset of **20,000 users** is generated.

Each user is randomly assigned to:

- Control group
- Treatment group

We simulate user behavior based on different conversion probabilities.

---

### 3. Exploratory Data Analysis

We examine:

- number of users in each group
- number of conversions
- conversion rates

---

### 4. Conversion Rate Comparison

We calculate the difference between control and treatment groups.

This difference is called **lift**.

Lift = Treatment Conversion − Control Conversion


---

### 5. Hypothesis Testing

A **Two-Proportion Z-Test** is used to determine whether the difference in conversion rates is statistically significant.

Hypotheses:

Null Hypothesis (H₀)

There is no difference between the two versions.


Alternative Hypothesis (H₁)

The new version changes the conversion rate.


If the p-value is less than **0.05**, the result is considered statistically significant.

---

### 6. Confidence Interval

A **95% confidence interval** is calculated to estimate the possible range of improvement.

This helps understand how large the real improvement might be.

---

### 7. Sample Ratio Mismatch (SRM) Check

This check ensures that users were split correctly between groups.

Example expected split:

50% control
50% treatment


If the traffic split is incorrect, the experiment results may be invalid.

---

### 8. Peeking Simulation

This simulation demonstrates the **peeking problem**.

Peeking happens when analysts check experiment results too early and stop the experiment prematurely.

This can increase the chance of **false positives**.

The project visualizes how p-values change over time during the experiment.

---

### 9. Visualization

Charts are created to visualize:

- conversion rate comparison
- p-value changes during the experiment

These visualizations help interpret experiment results more clearly.

---

# Example Result

Control Conversion Rate: 8.4%
Treatment Conversion Rate: 9.7%

Lift: +1.3%

P-value: 0.002


Conclusion:

The treatment significantly improves the conversion rate.


This means the new website design performs better and may be deployed.

---

# Tools Used

- Python
- Pandas
- NumPy
- SciPy
- Statsmodels
- Matplotlib

---

# Skills Demonstrated

This project demonstrates several important data science skills:

- statistical hypothesis testing
- experimental design
- data analysis
- statistical inference
- experiment validation
- data visualization

---

# Future Improvements

Possible extensions for this project:

1. Run **multiple experiments simultaneously** instead of analyzing only one experiment.
2. Add **guardrail metrics** such as bounce rate, session duration, or page load time.
3. Build an **automated experiment reporting dashboard**.
4. Integrate **real datasets** from product analytics platforms.
5. Implement **Bayesian A/B testing methods**.
6. Add a **web interface to simulate experiments interactively**.
7. Track **daily experiment metrics automatically**.

---

# Conclusion

This project demonstrates how A/B testing helps companies make **data-driven product decisions**.

Instead of guessing which product change is better, companies can run controlled experiments and use statistical analysis to identify the best option.
