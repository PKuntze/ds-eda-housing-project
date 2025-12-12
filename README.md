# Data Science EDA Housing Project

This project was done as part of the practical training during the Data Science, Machine Learning, and AI bootcamp by neuefische.
The main training point of the exercise was the general workflow of a data science project focused on Exploratory Data Analysis (EDA).
The timeframe that was given to accomplish this was 2 1/2 days.

## :clipboard: Project overview

We had to asume we are a consultant working for a business client who wants to sell or buy houses depending on their particular situation. We could chose from a list of fictional clients ourselfs.
The task was to analyse a data set containing information about the Seattle housing market roughly from May 2014 to May 2015, then come up with recommendations. The presentation was given in front of our bootcamp group.

The Client chosen here is Amy Williams, a Mafiosi who wants to sell several high value assets in central Seattle over time for profit. At the same time they are looking for average outskirt houses to hide from the FBI from time to time. The role chosen during the presentation was that of a conultant who is in on the criminal dealings.

The analysis of the data set was done in two parts.
1. Comming up with a strategy how to sell the central houses for the most profit. Theirby the key aspect turned out to be timing.
2. Finding the most suitable neighborhoods (represented by ZIP codes) in King County for hiding from the FBI. For this, additional internet research was done to classify the neighborhoods in regard to public sourveillance, accessibility and geagraphical area type (urban/rural).

Due to the lack of time for this project, an LLM was used to help come up with the clasification of the neighborhoods. All three characteristics have superficially been double checked and slightly adjusted. However, the clasifications do not claim to be accurate. For the scope of this project this was sufficient.

🔑 **Key Elements**:

- Comming up with research questions corresponding to the clients needs and at least three a priori hypotheses regarding the King County housing data set
- general EDA of the data set and verification of the hypotheses
- EDA focusing on the development of prices of top 10% assets in central Seattle
- Internet research and classification of the King County neighborhoods
- EDA focusing on finding suitable houses in suitable neighborhoods
- Taking on the role of a consultant and presenting the findings to the client and the company we work for



---

## 📂 Repository Structure
<details>
  <summary>Structure Visualization</summary>
    
  ```
project-name/
├── README.md                   <- Project overview and usage
├── requirements.txt            <- Main Python dependencies
├── .gitignore                  <- Ignored files for git
├── LICENSE                     <- Copyright license by neuefische GmbH
│
├── data/
│   ├── zip_codes_wa/           <- Shapefile used for plotting geographical data
│   ├── eda.csv                 <- Unchanged data set fetched from database
│   ├── sales.csv               <- Cleaned data set
│   └── zip_codes_*.csv         <- List of categorized ZIP codes from King country
│
├── notebooks/                  <- Notebooks containing EDA project solution
│   ├── templates/              <- Templates provided by DS bootcamp
│   ├── 1_Fetch_and_skim_data.ipynb
│   ├── 2_Explore_and_clean_data.ipynb
│   ├── 3_Additional_external_data.ipynb
│   ├── 4_Plot_Results.ipynb
│   └── EDA_project_notes.txt
│
├── optional/                   <- Tutorials provided by DS bootcamp
│
├── project_description/        <- Explanations and task description provided by DS bootcamp
│   ├── README.md               <- Information about environment setup
│   ├── assignment.md
│   ├── column_names.md
│   └── workflow.md
│
└── reports/
    ├── images/
    └── Presentation.pdf
  ```
</details>

### Data

The data is collected from the postgres database. The connection is set up in a .env file, which is not provided with this repository.

### Notebooks 
- `1_Fetch_and_skim_data.ipynb` - getting the data from the postgres database, having a first look at the data to get familiar.  
- `2_Explore_and_clean_data.ipynb` - data exploration and cleaning (if neccessary), accessing the development of central Seattle house prices.  
- `3_Additional_external_data.ipynb` - analysing and visualising King County in regard to the characteristics of the neighborhoods, finding most suitable ones.  
- `4_Plot_Results.ipynb` - analysing the data to find average low profile houses within the suitable neighborhoods.

### Optional

Can completely be disregarded.

### Project Description
- `assignment.md` - Everything about this Project.
- `olumn_names.md` - Describes the columns in the original data set.
- `workflow.md` - Project workflow tutorial.

### Reports
- `Presentation.pdf` - Presentation sumarizing project results, held during the DS bootcamp.



---

## ⚙️ Setup

Follow these steps to set up and run the project locally.

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

### 2. Create a virtual environment

Recommended Python version 3.11.3

```bash
python -m venv .venv

# Activate environment
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate     # Windows
```

### 3. Install dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```



---

## 📌 Notes

- `src/` contains the authoritative code for reproducibility.  
- `notebooks/` are explanatory and showcase data preparation, EDA, and baseline results.  
- Raw data should **not** be committed to GitHub.



---

## 🤝 Acknowledgements

- This work was done under the capstone project of the "Data Science, Machine Learning, and AI" bootcamp by [neuefische GmbH](https://www.neuefische.de).



---

## ✨ Authors

- Patrick Kuntze
