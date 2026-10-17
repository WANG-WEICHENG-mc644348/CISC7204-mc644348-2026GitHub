# CISC7204 — Data Science and Data Visualization

Coursework repository for **CISC7204 Data Science and Data Visualization**,
MSc in Data Science, University of Macau.

**WANG Weicheng** · mc644348 · mc64434@um.edu.mo

---

## Contents

| Folder | Assignment | Artifacts |
|:--|:--|:--|
| [`cisc7204-Assgn01-2026-mc644348/`](cisc7204-Assgn01-2026-mc644348/) | Assignment 01 | Modules 01–06 · 14 notebooks · 179 screenshots · preliminary project proposal |
| [`cisc7204-Assgn02-2026-mc644348/`](cisc7204-Assgn02-2026-mc644348/) | Assignment 02 | Modules 01–05 · 15 notebooks · 303 screenshots · shared datasets · project proposal |

Each assignment folder follows the same layout:

```
cisc7204-AssgnNN-2026-mc644348/
├── README.md                 module index for this assignment
├── Module 01/
│   ├── Lab01/                notebook + its screenshots
│   └── Lab02/
├── ...
├── Datasets/                 (Assignment 02 only) shared input data
└── Project Proposal/         project design, data and figures
```

---

## Assignment 01 — Data analysis with Python

Progresses from data import to modelling.

| Module | Topic |
|:--|:--|
| 01 | Importing datasets |
| 02 | Data wrangling |
| 03 | Exploratory data analysis |
| 04 | Model development |
| 05 | Model evaluation and refinement |
| 06 | Practice project (insurance cost analysis) and final project |

The `Project Proposal/` folder holds the preliminary proposal for the
course project, *Measuring Change in Judicial Trust in China: A Two-Wave
Analysis of the Chinese General Social Survey (2017 & 2023)*, together with
the working data and notebook.

## Assignment 02 — Data visualisation

Covers the standard plotting stack in Python, from Matplotlib to Plotly and
Folium.

| Module | Topic |
|:--|:--|
| 01 | pandas selection, filtering and sorting; Matplotlib basics; line plots |
| 02 | Area, histogram, bar, pie, box, scatter and bubble charts; subplots |
| 03 | Waffle charts, word clouds, Seaborn and regression plots; Folium, markers and choropleth maps |
| 04 | Plotly basics and Plotly Express; practice with an airline dataset |
| 05 | Practice project (historical wildfires) and final project (automobile sales) |

The `Project Proposal/` folder holds the project design for the second half
of the course, developed from the same CGSS study.

---

## Reproducing the notebooks

Every notebook is committed **with its outputs saved**, so results can be
read directly on GitHub without running anything.

To re-run:

```bash
pip install -r cisc7204-Assgn02-2026-mc644348/requirements.txt
jupyter lab
```

Assignment 02 notebooks read their inputs as `Datasets/<file>`, i.e. the
paths are relative to the assignment root. Launch Jupyter from inside
`cisc7204-Assgn02-2026-mc644348/` (or move the notebook there temporarily)
so those paths resolve.

Assignment 01 notebooks use the small CSV files that sit beside them in the
same `Lab` folder.

## Notes

- Screenshots are the evidence submitted to the course forum for each lab;
  they are grouped in the same folder as the notebook that produced them.
- `Datasets/` contains the teaching datasets distributed with the course.
- Any personal, credential or restricted material is deliberately excluded.
