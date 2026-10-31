# SmartMessage AI

### SMS Spam Detection System

## Overview

SmartMessage AI is a machine learning project that aims to develop a system capable of automatically classifying SMS messages as **Spam** (unwanted messages) or **Ham** (legitimate messages).

The project explores the different stages of building a text classification system, from data exploration and preprocessing to model development and evaluation.

## Objectives

- Explore and understand SMS datasets.
- Perform data cleaning and preprocessing using Python.
- Apply Natural Language Processing (NLP) techniques.
- Develop and evaluate machine learning classification models.
- Build a system capable of identifying unwanted messages.

## Dataset

The project uses the **SMS Spam Collection** dataset provided by the UCI Machine Learning Repository.

- **Source:** [UCI Machine Learning Repository – SMS Spam Collection](https://archive.ics.uci.edu/dataset/228/sms+spam+collection)
- **Number of messages:** 5,574
- **Language:** English
- **Classification labels:**
  - `ham`: legitimate messages.
  - `spam`: unwanted messages.

The original dataset is preserved in its raw format. A processed version is also available for data exploration and preparation.

## Technologies & Tools

- **Programming language:** Python
- **Data manipulation:** Pandas
- **Data visualization:** Matplotlib
- **Development environment:** Jupyter Notebook, Visual Studio Code
- **Version control:** Git and GitHub

## Project Structure

```text
SmartMessage_AI/
│
├── data/
│   ├── raw/
│   │   └── SMSSpamCollection
│   │
│   └── processed/
│       └── sms_spam_collection.csv
│
├── notebooks/
│   ├── W01_python.ipynb
│   ├── W02_pandas.ipynb
│   └── W03_dataset_audit.ipynb
│
├── reports/
│   └── dataset_profile.md
│
├── messages.csv
├── README.md
├── LEARNING_JOURNAL.md
└── .gitignore
```

## Project Status

This project is currently under development. Data exploration and preparation are being carried out before moving on to machine learning model development.

## Author

**Rania Hafa**