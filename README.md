#  Pet Adoption Analysis: Uncovering Patterns in Shelter Outcomes

This project analyzes shelter animal intake and outcome data to identify the key factors that influence whether an animal gets adopted. Using logistic regression, decision trees, and random forest models, it reveals patterns that can help shelters improve adoption strategies and reduce return rates.

---

##  Project Summary

Animal shelters face challenges with overcrowding, limited resources, and high return rates. This project explores patterns in adoption outcomes by analyzing structured data on animal characteristics, intake reasons, and movement types(adopted/ notadopted).

**Main Goals:**
- Determine which features (age, breed, species, etc.) most influence adoption outcomes
- Predict the likelihood of adoption using machine learning models
- Provide actionable insights for shelters to optimize their adoption processes

  ##  Tools & Technologies

- **Languages**: R

  ## 📂 Dataset Description

This project uses real-world animal shelter data to uncover patterns in pet adoption outcomes. The dataset was obtained from [Shelter Pet Data Alliance](https://www.shelterpetdata.org/) and contains detailed intake and outcome records from a municipal shelter.

###  Key Columns in the Dataset

- `speciesname` – Animal species (e.g., Dog, Cat, Rabbit)
- `breedname` – Breed or breed mix
- `age_years` – Age at intake (in years)
- `sexname` – Sex of the animal (Male, Female, Unknown)
- `intakereason` – Reason for intake (Owner surrender, Stray, etc.)
- `movementtype` – Outcome (Adopted, Returned, Euthanized)
- `movementdate` – Outcome date
- `istransfer` – Boolean indicating if animal was transferred
- `sheltercode` – Shelter identifier
- `animalname` – Name if assigned

###  Database Structure

While the project uses a single flat CSV file, it reflects the structure of a normalized relational database. In production, this data would likely be split into related tables:

- `animals`: Static info like species, age, and breed
- `intakes`: Each intake event (reason, date, source)
- `outcomes`: Each outcome event (type, date)
- `shelters`: Shelter metadata

This structure enables queries such as:
- Adoption rates by breed and age
- Return rates by intake reason
- Time-in-shelter by species or outcome type

###  [Click here to view the dataset](animal-data-1.csv)



###  Top 10 Adopted Dog Breeds
![Top 10 Adopted Dog Breeds](adopted%20dog%20breeds.jpeg)

###  Adoption Counts by Age
![Adoption Counts by Age](age%20counts.jpeg)

###  Decision Tree Model
![Decision Tree](tree.jpeg)

###  Random Forest Feature Importance
![Random Forest](random%20forest.jpeg)

###  ROC Curve
![ROC Curve](roc%20curve.jpeg)

###  Return Reasons for Returned Pets
![Return Reasons](return%20final.jpeg)

###  Dog Euthanasia in 2023
![Dog Euthanasia](dog%202023%20euthanased.jpeg)

### ♂ Adoption Likelihood by Gender
![Adoption by Gender](gender.jpeg)

###  Most Popular Dog Breeds in Shelter
![Top Dog Breeds](top%20dog%20breeds.jpeg)
