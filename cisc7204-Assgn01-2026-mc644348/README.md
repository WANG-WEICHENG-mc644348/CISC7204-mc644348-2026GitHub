# CISC7204 — Assignment 01

**WANG Weicheng** · mc644348 · mc64434@um.edu.mo

Data analysis with Python: from importing a dataset to fitting and refining a
model, ending with a practice and a final project.

All notebooks are committed **with outputs saved**, so every result is
readable on GitHub without running the code.

---

## Module index

| Module | Lab | Topic | Notebook | Screenshots |
|:--|:--|:--|:-:|:-:|
| 01 | Lab01 | Importing a dataset | 1 | 13 |
| 01 | Lab02 | Practice — laptops pricing | 1 | 6 |
| 02 | Lab01 | Data wrangling | 1 | 23 |
| 02 | Lab02 | Practice — data wrangling | 1 | 12 |
| 03 | Lab01 | Exploratory data analysis | 1 | 20 |
| 03 | Lab02 | Practice — laptops pricing | 1 | 15 |
| 04 | Lab01 | Model development | 1 | 18 |
| 04 | Lab02 | Practice — model development | 1 | 10 |
| 05 | Lab01 | Model evaluation and refinement | 1 | 23 |
| 05 | Lab02 | Practice — model evaluation | 1 | 11 |
| 06 | Practice project | Insurance cost analysis | 1 | 13 |
| 06 | Final Project | Course final project | 2 | 15 |

Each `Lab` folder contains one notebook and the screenshots that document
each step of the exercise. Small CSV inputs sit in the same folder as the
notebook that reads them.

## Project Proposal

`Project Proposal/` holds the preliminary proposal for the course project:

> **Measuring Change in Judicial Trust in China: A Two-Wave Analysis of the
> Chinese General Social Survey (2017 & 2023)**

| File | Description |
|:--|:--|
| `CGSS_judicial_trust_workflow.ipynb` | Working notebook: harmonising the two waves and first descriptive results |
| `CGSS2017_2023_pooled_python.csv` | Pooled two-wave dataset |
| `CGSS2017_cleaned_reference.csv` | Cleaned 2017 wave |
| `CGSS2023_cleaned_python.csv` | Cleaned 2023 wave |

The written proposal itself was submitted through the course site and is not
duplicated here; the study design is summarised in
[`Project Proposal/README.md`](Project%20Proposal/README.md).

The project is a two-member collaboration with LI Siwei (MC638482).

---

## Running

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
jupyter lab
```

Open any notebook in its own folder; the CSV inputs are alongside it.
