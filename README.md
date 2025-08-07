#  Pet Adoption Analysis: Uncovering Patterns in Shelter Outcomes

This project analyzes shelter animal intake and outcome data to identify the key factors that influence whether an animal gets adopted. Using logistic regression, decision tree, and random forest models, it reveals patterns that can help shelters improve adoption strategies and reduce return rates.

---

> In 2023 alone, **California and Texas euthanized over 40,000 dogs** due to high rates of animal surrender, overcrowded shelters, and insufficient funding (as shown in the chart below).

![Dog Euthanasia](dog%202023%20euthanased.jpeg)

##  Main Goals

- Identify features (age, breed, species, etc.) that most influence adoption outcomes  
- Predict the likelihood of adoption using machine learning models  
- Provide actionable insights to help shelters optimize adoption processes  

---

##  Project Overview

- Focused on **dogs only**
- Cleaned and preprocessed **30,000+ records**
- Explored variables including **breed, age, sex, intake reason, and adoption outcome**
- Built predictive models:  
  - Logistic Regression  
  - Decision Tree  
  - Random Forest
- Created visualizations to highlight trends and key findings

---
# Language 
R was primarlity used in cleaning and manipulating the dataset


##  Data Source

- Shelter Pet Data Alliance  
- Nationwide data, updated monthly  
- Uploaded directly by U.S. shelters

  ###  [Click here to view the dataset](animal-data-1.csv)

##  Dataset Schema


| **Column**           | **Description**                                                 |
|----------------------|-----------------------------------------------------------------|
| `id`                 | Unique animal intake ID                                         |
| `intakedate`         | Date animal entered the shelter                                 |
| `intakereason`       | Reason for intake (e.g., Moving, Abandoned)                     |
| `istransfer`         | 1 if animal was transferred from another facility               |
| `sheltercode`        | Internal shelter code                                           |
| `identichipnumber`   | Microchip or unique ID                                          |
| `animalname`         | Name of the animal                                              |
| `breedname`          | Animal's breed                                                  |
| `basecolour`         | Base color of the animal                                        |
| `speciesname`        | Cat or Dog                                                      |
| `animalage`          | Age at time of intake                                           |
| `sexname`            | Sex (e.g., Male, Female)                                        |
| `location`           | Area of the shelter the animal was housed in                   |
| `movementdate`       | Date the animal left the shelter or moved within it            |
| `movementtype`       | Type of movement (Adoption, Foster, etc.)                       |
| `istrial`            | Indicates if the movement was part of a trial                   |
| `returndate`         | If returned, the date they were returned                        |
| `returnedreason`     | Reason for return (if applicable)                               |
| `deceaseddate`       | Date of death (if applicable)                                   |
| `deceasedreason`     | Reason for death (e.g., died in care)                           |
| `diedoffshelter`     | 1 if death occurred off-shelter                                 |
| `puttosleep`         | 1 if euthanized                                                 |
| `isdoa`              | 1 if dead on arrival                                            |

---

##  Interactive Shiny App

Explore the interactive version of this project through the Shiny web application:

 **[Click here to launch the app](https://britt1996.shinyapps.io/adoption_app_v2/)**

This Shiny app allows users to:

- View adoption likelihood by **age**, **breed**, and **gender**
---


### Results and Discussion:


###  Return Reasons for Returned Pets

- Dogs surrendered due to **housing issues** or **behavioral concerns** had lower chances of successful adoption.
- Return rates were higher for dogs adopted **without proper breed research or preparation**.

![Return Reasons](return%20final.jpeg)


###  Most Popular Dog Breeds in Shelter

- The most common breeds were often **stigmatized breeds** or **high-energy dogs**.
![Top Dog Breeds](top%20dog%20breeds.jpeg)

###  Adoption Counts by Age
- Adoption rates **decline with age**.
- Puppies are adopted at significantly higher rates than older dogs.
![Adoption Counts by Age](age%20counts.jpeg)


###  Decision Tree Model
- **Age** was the strongest predictor of adoption.
- Dogs under 3 years old were adopted more quickly.
- Breed had less impact than expected.
- Senior dogs were more likely to remain in shelters or face euthanasia.
- 
![Decision Tree](tree.jpeg)

###  Random Forest Feature Importance
- Had the **highest accuracy** of all models.
- Feature importance plot confirmed that **age** and **breed** were top predictors.
  
![Random Forest](random%20forest.jpeg)

###  ROC Curve
- Logistic regression provided a solid **baseline prediction model**.
- Both **age** and **breed** were statistically significant predictors.
- ROC curve showed strong performance distinguishing adopted vs. non-adopted cases.
![ROC Curve](roc%20curve.jpeg)

### Adoption Likelihood by Gender
- Sex-based trends showed minor differences.
- In some cases, **female dogs** were slightly more likely to be adopted.
![Adoption by Gender](gender.jpeg)

##  Contact

For questions, feedback, or collaboration opportunities, feel free to connect with me via [GitHub](https://github.com/Britt1996).

