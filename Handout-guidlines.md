# Data Science and Machine Learning
## Group Project 2025/2026  
### Reach for Change  
### Part 1: Uncovering Donor Profiles Through Clustering

*MARCH, 2026*

---

## I. INTRODUCTION

In recent years, nonprofit organizations have faced an unexpected challenge.  
While the number of charitable causes has grown significantly, people’s tolerance for repeated solicitations has decreased. Many potential supporters report feeling overwhelmed by generic fundraising campaigns, leading to lower engagement and long-term disengagement from charitable initiatives.

To address this issue, the **Civic Support Alliance (CSA)**, a federation representing multiple humanitarian and social aid programs, has decided to modernize how outreach campaigns are conducted.

Instead of contacting everyone in their database, the organization wants to better understand the different types of individuals within their supporter base. The objective is not only operational efficiency but also respect: communicating in ways that are more relevant, more personalized, and better aligned with people’s profiles and past behavior.

The CSA has accumulated historical data from previous fundraising campaigns, including demographic information, past interaction history, and donation behavior. They have provided a dataset containing individuals who may be contacted in an upcoming campaign. However, before building predictive tools, the organization first needs **a clearer picture of who these individuals are**.

Your team has been hired as a group of data scientists to conduct an exploratory segmentation study. Your goal is to use **clustering techniques to identify meaningful groups of individuals within the dataset**.

By uncovering distinct supporter profiles, you will help the organization understand the structure of its donor base and lay the foundation for more informed and targeted outreach strategies.

---

## II. PROJECT GOALS

The primary components and goals of the project are:

1. **Preprocessing and Exploratory Data Analysis (EDA)**  
   Clean and preprocess your dataset, performing an exploratory analysis to uncover patterns and relationships.

2. **Clustering**  
   Identify and analyze reasonable segments with **at least two perspectives**.  
   You must:
   - Choose different features for each segment  
   - Implement clustering models  
   - Tune and evaluate them  
   - **Report all findings**  
   - Choose the approach that makes the most sense  
   - Provide a **critical assessment**

   Focus on segmenting the population, analyzing the key features that define each group and understanding what differentiates them.  
   This should be accompanied by **a preliminary action plan** to guide future initiatives.

---

## III. DATASET

You have access to **one dataset**:

- **`donors_train.csv`**  
  Contains features that give detailed information about each possible donor.

### Available Attributes

| Attribute | Description |
|---------|------------|
| **CONTROL_NUMBER** | Unique identifier of each possible donor |
| **DONOR_AGE** | Age as of last year's mail solicitation |
| **URBANICITY** | Nature of the donor's location (U = Urban, C = City, T = Town, R = Rural, S = Suburban) |
| **SES** | Socioeconomic status code (5 profiles) |
| **HOME_OWNER** | H if homeowner, U if unknown |
| **DONOR_GENDER** | Gender of individual |
| **INCOME_GROUP** | Income group code (7 levels) |
| **WEALTH_RATING** | Wealth rating code (10 levels) |
| **MEDIAN_HOME_VALUE** | Median home value (in $100s) |
| **MEDIAN_HOUSEHOLD_INCOME** | Median household income (in $100s) |
| **PCT_OWNER_OCCUPIED** | % of owner-occupied housing nearby |
| **PER_CAPITA_INCOME** | Per capita income of neighborhood |
| **PCT_ATTRIBUTE1** | % male active military nearby |
| **PCT_ATTRIBUTE2** | % male veterans nearby |
| **PCT_ATTRIBUTE3** | % Vietnam veterans nearby |
| **PCT_ATTRIBUTE4** | % WW2 veterans nearby |
| **PEP_STAR** | STAR donor status (3 consecutive campaigns) |
| **RECENT_STAR_STATUS** | STAR achieved in the last 4 years |
| **CHILDREN** | Number of children |
| **RECENT_AVG_GIFT_AMT** | Average donation in the last 4 years |
| **RECENT_CARD_RESPONSE_PROP** | Number of card responses in the last 4 years |

---

### Additional Attributes

| Attribute | Description |
|---------|------------|
| **RECENCY_STATUS_96NK** | Donor status: A (active), E (inactive), F (first time), L (lapsing), N (new), S (star) |
| **FREQUENCY_STATUS_97NK** | Number of donations in the relevant period |
| **RECENT_RESPONSE_PROP** | Response proportion over solicitations |
| **FILE_CARD_GIFT** | Lifetime average donation to card solicitations |
| **LIFETIME_CARD_PROM** | Total number of card promotions sent |
| **LIFETIME_PROM** | Total promotions sent |
| **RECENT_AVG_CARD_GIFT_AMT** | Average card donation in last 4 years |
| **RECENT_RESPONSE_COUNT** | Responses to any promotion in last 4 years |
| **RECENT_CARD_RESPONSE_COUNT** | Card responses in last 4 years |
| **MONTHS_SINCE_LAST_PROM_RESP** | Months since last response |
| **LIFETIME_GIFT_AMOUNT** | Total lifetime donation amount |
| **LIFETIME_GIFT_COUNT** | Total number of donations |
| **LIFETIME_MAX_GIFT_AMT** | Maximum donation |
| **LIFETIME_MIN_GIFT_AMT** | Minimum donation |
| **LAST_GIFT_AMT** | Most recent donation amount |
| **CARD_PROM_12** | Card promotions in last 12 months |
| **NUMBER_PROM_12** | Total promotions in last 12 months |
| **MONTHS_SINCE_LAST_GIFT** | Months since last donation |
| **MONTHS_SINCE_FIRST_GIFT** | Months since first donation |

---

## IV. DELIVERABLES

By the project deadline, you must submit:

- **Jupyter Notebook(s)** (or a ZIP file):
  - All code used to make decisions and obtain results
  - Non-essential decision code should be **included but commented**
  - Naming format: `DSML_GroupXX`

- **PDF of the Notebook(s)**:
  - Without outputs
  - Maximum **25 A4 pages**
  - Each extra page: **−0.5 values**
  - Naming format: `DSML_GroupXX_pdf`

---

## V. EVALUATION

- Late submissions:
  - Up to **3 days late**: −1 point per day
  - After 3 days: **not accepted**

**Deadline:** **May 4th, 2026 – 18:00**

### Grading Breakdown

| Criteria | Weight (%) | Max Grade (20) |
|--------|------------|----------------|
| Project Structure & Notebook Quality | 20 | 4 |
| Preprocessing & EDA | 25 | 5 |
| Modeling & Results | 40 | 8 |
| Action Plan | 5 | 1 |
| Creativity and Self‑Study | 10 | 2 |

---

## V. GRADING DETAILS

### Project Structure & Notebook Quality (4)
- Clarity and readability
- Clear goals and structure
- Appropriate techniques
- Highlighted insights and implications

### Preprocessing & EDA (5)
- Dataset understanding
- Relevant insights
- Data cleaning, transformation, and reduction
- Feature creation with justification

### Modeling & Results (8)
- At least **two clustering perspectives**
- Feature selection explanation
- Statistical and visual cluster analysis

### Action Plan (1)
- Clear and actionable recommendations for CSA

### Creativity and Self‑Study (2)
- Use of additional techniques
- Theoretical explanation when required

---

## VI. PARTING NOTES

- The notebook is the **only evaluation artifact**
- Keep it concise and focused
- Avoid long theory explanations already covered in class
- Run the notebook **from start to finish** before submission
- Include unused code, but ensure it is **commented**
- Notebooks must run in one go, or penalties apply
- Work will be compared across groups

### Friendly Reminders
- If it’s worth mentioning, include it wisely
- **Finished is better than perfect**