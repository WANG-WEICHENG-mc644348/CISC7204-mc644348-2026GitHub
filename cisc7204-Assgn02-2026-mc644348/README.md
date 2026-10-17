# CISC7204 — Assignment 02

**WANG Weicheng** · mc644348 · mc64434@um.edu.mo

Data visualisation in Python: Matplotlib, Seaborn, Folium and Plotly, built
up module by module and finished with two open-ended projects.

All notebooks are committed **with outputs saved**, so every chart is
readable on GitHub without running the code.

---

## Module index

| Module | Lab | Topic | Notebook | Screenshots |
|:--|:--|:--|:-:|:-:|
| 01 | Lab01 | Import and data overview; selecting columns and rows; filtering; sorting | 1 | 39 |
| 01 | Lab02 | pandas refresher; Matplotlib and pyplot basics; line plots | 1 | 15 |
| 02 | Lab01 | Importing libraries and fetching data; area plots; histograms; bar charts | 1 | 30 |
| 02 | Lab02 | Visualising with Matplotlib; pie, box, scatter and bubble charts | 1 | 32 |
| 02 | Lab03 | Line, scatter, bar, histogram and pie charts; sub-plotting | 1 | 31 |
| 03 | Lab01 | Waffle charts; word clouds; Seaborn; regression plots | 1 | 43 |
| 03 | Lab02 | Folium; maps with markers; choropleth maps | 1 | 22 |
| 04 | Lab01 | Plotly basics; Plotly Express; practice with an airline dataset | 1 | 26 |
| 04 | Lab02 | Plotly practice exercises | 1 | 4 |
| 04 | Lab03 | Plotly practice exercises | 1 | 5 |
| 04 | Lab04 | Plotly practice exercises | 1 | 6 |
| 05 | Practice Lab01 | Practice project — historical wildfires | 1 | 17 |
| 05 | Practice Lab02 | Practice project — continued | 1 | 6 |
| 05 | Final Lab01 | Final project — automobile sales | 1 | 16 |
| 05 | Final Lab02 | Final project — continued | 1 | 11 |

Each `Lab` folder contains the notebook for that exercise together with the
screenshots that document it. Screenshots follow the naming convention
`A02_M<module>_<lab>_<step>_<description>.png`.

## Datasets

Shared inputs live in [`Datasets/`](Datasets/). They are the teaching
datasets distributed with the course.

| File | Used in |
|:--|:--|
| `Canada.csv`, `Canada.xlsx` | Modules 01–03 |
| `alice_novel.txt`, `alice_mask.png` | Module 03 (word clouds) |
| `Police_Department_Incidents_-_Previous_Year__2016_.csv` | Module 03 (choropleth) |
| `us-states.json`, `world_countries.json` | Module 03 (maps) |
| `airline_data.csv` | Module 04 |
| `automobile-sales.csv` | Module 05 final project |
| `Historical_Wildfires.csv` | Module 05 practice project |

## Project Proposal

[`Project Proposal/`](Project%20Proposal/) holds the design for the course
project, which continues the CGSS judicial-trust study begun in
Assignment 01. See its [README](Project%20Proposal/README.md) for scope and
what is deliberately not published.

---

## Reproducing

```bash
pip install -r requirements.txt
jupyter lab
```

**Working directory matters.** Notebooks open their inputs with paths such
as `Datasets/Canada.csv`, i.e. relative to this assignment folder. To re-run
one, either launch Jupyter from inside `cisc7204-Assgn02-2026-mc644348/` and
open the notebook from there, or copy the notebook to this folder first.

Module 03 Lab02 uses a 31 MB incident-level CSV and Module 04 Lab01 includes
many embedded Plotly outputs, so those two notebooks are large; they render
fine on GitHub but may take a moment to open.
