# Module_5

# Coupon Acceptance Analysis

## Overview
This project explores the factors that influence whether drivers accept coupons while driving, with a particular focus on **Coffee House** and **Bar** coupons. Using exploratory data analysis (EDA) and subgroup comparisons, the analysis investigates how **behavioral context, demographics, travel constraints, and social factors** affect coupon acceptance.

The dataset contains information about drivers’ destinations, passengers, income, age, frequency of visiting certain venues, weather conditions, and whether the offered coupon was accepted.

---

## Objectives
The primary goals of this project are to:

- Understand overall coupon acceptance behavior
- Identify which driver characteristics are associated with higher acceptance rates
- Examine how contextual factors (e.g., destination, distance, temperature) influence acceptance
- Explore differences in acceptance rates for Coffee House coupons across:
  - Travel time to the coupon location
  - Passenger type (alone, adult passenger, child passenger)
  - Gender
  - Destination
  - Temperature
- Form behavioral hypotheses about drivers most likely to accept coupons

---

## Dataset
- **Source:** Coupon acceptance dataset (survey-based)
- **Observations:** ~12,000+
- **Key columns include:**
  - `coupon` – type of coupon offered
  - `Y` – coupon accepted (1) or not accepted (0)
  - `temperature`
  - `destination`
  - `passanger`
  - `gender`
  - `age`
  - `income`
  - `toCoupon_GEQ5min`, `toCoupon_GEQ15min`, `toCoupon_GEQ25min`
  - Venue frequency variables (e.g., `Bar`, `RestaurantLessThan20`)

---

## Methods
The analysis follows a structured exploratory workflow:

### 1. Data Understanding & Quality Checks
- Inspected data types and structure
- Verified absence of missing or duplicate values
- Validated categorical and binary fields
- Confirmed logical consistency of key variables

### 2. Exploratory Data Analysis (EDA)
- Computed acceptance rates using the mean of the binary target variable (`Y`)
- Compared acceptance rates across meaningful subgroups
- Created bar plots and histograms to visualize patterns
- Evaluated contextual factors such as distance, destination, and temperature

### 3. Subgroup Comparisons
Examples include:
- Bar coupon acceptance by bar visitation frequency
- Coffee House acceptance by travel time
- Coffee House acceptance by passenger type
- Acceptance differences by gender and destination
- Combined conditions using logical AND / OR criteria

### 4. Hypothesis Development
Patterns observed in the data were used to develop behavioral hypotheses about coupon acceptance rather than to make causal claims.

---

## Key Findings
- Coupon acceptance is **strongly associated with existing behavior** (e.g., frequent bar or restaurant visits).
- **Proximity matters**: acceptance decreases as required travel time increases.
- Coffee House coupons are more likely to be accepted when drivers:
  - Are traveling alone
  - Have no urgent destination
  - Experience warmer temperatures
- Social context (presence of children, marital status) influences acceptance behavior.
- Coupons tend to **reinforce existing habits** rather than change behavior.

---

## Technologies Used
- Python
- pandas
- matplotlib
- seaborn
- statsmodels (for optional statistical testing)

---

## Repository Structure
