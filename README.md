
# Chi-Square Test Coding Questions (with Datasets)

---

###  1. Gender vs Purchase Decision

**Business Context:**
A marketing team is analyzing whether gender influences the likelihood of purchasing a product.

**Goal:**
Test if there’s a **statistically significant relationship** between a customer’s gender and whether they purchased the product.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
import pandas as pd

data = pd.DataFrame({
    'gender': ['Male', 'Male', 'Female', 'Female', 'Male', 'Female', 'Male', 'Female', 'Male', 'Female'],
    'purchased': ['Yes', 'No', 'Yes', 'No', 'Yes', 'Yes', 'No', 'No', 'Yes', 'No']
})
```

**Question:**
Is the purchase decision independent of gender?

---

### 2. Education Level vs Payment Method

**Business Context:**
An e-commerce platform wants to understand if educational background influences the choice of payment method at checkout.

**Goal:**
Find out if payment method (Credit, Debit, or Cash) is related to education level.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
data = pd.DataFrame({
    'education': ['High School', 'Bachelors', 'Masters', 'Bachelors', 'Masters', 'High School', 'Bachelors', 'Masters', 'High School', 'Bachelors'],
    'payment_method': ['Credit', 'Cash', 'Credit', 'Debit', 'Cash', 'Debit', 'Credit', 'Debit', 'Cash', 'Credit']
})
```

**Question:**
Is there a statistically significant association between education level and preferred payment method?

---

### 3. Fair Dice – Expected vs Observed Rolls

**Business Context:**
You roll a six-sided die 120 times to check if it’s fair.

**Goal:**
Test whether the observed counts deviate significantly from the expected equal distribution.

**Chi-Square Test Type:**
**Goodness-of-Fit Test**

**Data:**

```python
observed = [16, 22, 18, 19, 23, 22]  # Rolls for faces 1 to 6
expected = [20] * 6  # Expected count per face = 120 / 6
```

**Question:**
Is the die fair, or do some numbers appear more frequently than others?

---

### 4. Customer Complaints Across Regions

**Business Context:**
A telecom company received customer complaints from 4 regions. They suspect some regions complain more than others.

**Goal:**
Test if complaints are uniformly distributed across regions.

**Chi-Square Test Type:**
**Goodness-of-Fit Test**

**Data:**

```python
observed = [120, 100, 80, 150]  # East, West, North, South
expected = [112.5] * 4  # Total = 450 complaints → 112.5 expected per region
```

**Question:**
Are customer complaints uniformly distributed across all four regions?

---

### 5. Smoking vs Exercise Frequency

**Business Context:**
Health researchers are studying whether smokers and non-smokers differ in how often they exercise.

**Goal:**
Check for a relationship between smoking status and exercise frequency.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
data = pd.DataFrame({
    'smoker': ['Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No', 'Yes', 'No'],
    'exercise_freq': ['Daily', 'Weekly', 'Rarely', 'Daily', 'Weekly', 'Rarely', 'Weekly', 'Daily', 'Rarely', 'Weekly']
})
```

**Question:**
Is there a significant association between being a smoker and how frequently someone exercises?

---

###  6. Click-Through Rate vs Time of Day

**Business Context:**
A digital marketing analyst wants to know whether the time of day affects whether people click on ads.

**Goal:**
Determine if ad click-through behavior varies by time of day.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
data = pd.DataFrame({
    'time_of_day': ['Morning', 'Afternoon', 'Evening', 'Night', 'Morning', 'Afternoon', 'Evening', 'Night', 'Morning', 'Night'],
    'clicked_ad': ['Yes', 'No', 'Yes', 'Yes', 'No', 'No', 'Yes', 'No', 'Yes', 'No']
})
```

**Question:**
Is ad click-through rate independent of the time of day?

---

### 7. Favorite Genre vs Age Group

**Business Context:**
A streaming company wants to see if different age groups prefer different types of content.

**Goal:**
Evaluate if a person’s favorite genre is associated with their age group.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
data = pd.DataFrame({
    'age_group': ['Teen', 'Adult', 'Senior', 'Teen', 'Adult', 'Senior', 'Teen', 'Adult', 'Senior', 'Teen'],
    'genre': ['Action', 'Drama', 'Comedy', 'Drama', 'Comedy', 'Action', 'Action', 'Comedy', 'Drama', 'Comedy']
})
```

**Question:**
Is there a significant relationship between age group and favorite genre?

---

### 8. Returns by Product Category

**Business Context:**
A retail platform is tracking how often products are returned across categories.

**Goal:**
Test if return frequency is equal across different product categories.

**Chi-Square Test Type:**
**Goodness-of-Fit Test**

**Data:**

```python
observed = [35, 50, 45, 30]  # Electronics, Clothing, Books, Home
expected = [40, 40, 40, 40]
```

**Question:**
Is the number of product returns evenly distributed across the four product categories?

---

### 9. Election Poll – Expected vs Actual Votes

**Business Context:**
A political analyst wants to verify if the actual votes match the poll prediction.

**Goal:**
Compare observed vs expected votes for four candidates.

**Chi-Square Test Type:**
**Goodness-of-Fit Test**

**Data:**

```python
observed = [260, 230, 270, 240]  # Candidates A, B, C, D
expected = [250, 250, 250, 250]
```

**Question:**
Do actual vote results match what was predicted in the polls?

---

### 10. Marital Status vs Employment Status

**Business Context:**
A sociologist is researching whether employment status is influenced by marital status.

**Goal:**
Check if there is any association between marital status and employment status.

**Chi-Square Test Type:**
**Test of Independence**

**Dataset:**

```python
data = pd.DataFrame({
    'marital_status': ['Single', 'Married', 'Divorced', 'Married', 'Single', 'Divorced', 'Married', 'Single', 'Divorced', 'Single'],
    'employment_status': ['Employed', 'Unemployed', 'Retired', 'Employed', 'Retired', 'Employed', 'Retired', 'Unemployed', 'Unemployed', 'Employed']
})
```

**Question:**
Is employment status associated with marital status?

---

