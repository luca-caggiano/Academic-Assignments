# Econometrics Replication Projects
This repository serves as a centralized portfolio of econometric analyses  developed as part of my university course assignments. Each project represents a partial replication of academic papers I studied during the courses.


## ⚠️ Important Disclaimer
> **Please note that all theoretical approaches, research methods, data sets, and the choice of analysis techniques used in these projects are NOT my own work.** All intellectual property rights, hypotheses, and findings belong entirely to the authors of the corresponding papers mentioned in each project.

**The main purpose of these projects is improving my technical skills.** While the original university assignments required **Stata** to be completed, I voluntarily choose to replicate them using **Python** from scratch. Such a translation is used as an opportunity for the development of my coding and analytical skills.

**Only the source code and technical execution are entirely my own work.**


## 📂 Repository Structure
Each folder contains a distict assignment, consiting of: 
* A **Jupyter notebook** with all the source code and detailed explanations of the workflow
* A **README file** describing the central hypothesis, statistical techniques,and findings about each project.


> Please be aware that the theoretical explanations presented in markdown cells within the notebooks are merely summaries of the arguments provided by the authors in their respective articles. The only purpose of these interpretations is to help readers interpret the coefficients if they have not read the original paper.


### Devotion and Development (Squicciarini, 2020)
* **Topic:** Evaluating the interaction between religiosity, primary school curricula, and industrial development during the Second Industrial Revolution in France [cite: 4-8].
* **Core Tasks Replicated:** Multi-cohort panel analysis, Department/Cohort Fixed Effects, and alternative mechanism robustness checks (fertility and vaccination controls).
* **Folder:** `/Religion and economic development`

### The Colonial Origins of Comparative Development (Acemoglu, Johnson, & Robinson, 2001)
* **Topic:** Estimating the causal impact of institutional quality (property rights) on long-term modern economic development using historical European settler mortality as an instrumental variable.
* **Core Tasks Replicated:** Baseline OLS regressions with progressive geographic and continent controls, Instrumental Variable (IV-2SLS) estimation, First Stage instrument validation, and reduced-form visualization.
* **Folder:** `/The Colonial Origins of Comparative Development`

### How Do Voters Respond to Information? (Kendall et al., 2015)
* **Topic:** Assessing voter responsiveness to different campaign message types (valence vs. ideology) and delivery channels (phone vs. mail) using a Randomized Controlled Trial (RCT) design.
* **Core Tasks Replicated:** Ex-ante experimental balancing tests to validate randomization protocols, and aggregate/individual-level OLS regression modeling with clustered robust standard errors.
* **Folder:** `/Voters response to information`

## 🔒 Note on Data Availability
The datasets used in each assignment (`.dta` files) are excluded by the repository. The data was directly provided by the course professors for educational purposes. To respect academic integrity and potential data licensing constraints, I decided to include the Data folders in the `.gitignore` file.