# Project Proposal — Judicial trust in China (preliminary)

**WANG Weicheng** (mc644348) · **LI Siwei** (MC638482)
CISC7204 Data Science and Data Visualization, University of Macau

---

## Topic

**Measuring change in judicial trust in China: a two-wave analysis of the
Chinese General Social Survey (2017 & 2023).**

**Research question.** How did public trust in the judiciary change in China
between 2017 and 2023, which individual-level characteristics are associated
with judicial trust, and for which groups did trust change the most?

## Data

| Source | Content |
|:--|:--|
| CGSS 2017 | Nationally representative survey; judicial trust measured on an 11-point scale about **courts** |
| CGSS 2023 | Same series; judicial trust measured on a 4-point scale about **judges** |

Both waves are distributed by CNSDA as `.dta` files after registration:

- CGSS 2017 — <https://www.cnsda.org/index.php?r=projects/view&id=94525591>
- CGSS 2023 — <https://www.cnsda.org/index.php?r=projects/view&id=11256439>

After cleaning and keeping respondents with a valid answer to the
judicial-trust item, the analytical sample is roughly 3,950 (2017) and
5,540 (2023).

## The measurement problem

The two waves do not measure the same thing in the same way: the 2017 item
asks about trust in **courts** on an 11-point scale, the 2023 item asks about
trust in **judges** on a 4-point scale. Comparing the two raw means would
confound real change with a change of instrument.

The project therefore treats harmonisation as a first-class step and reports
several outcomes rather than one: a binary high-trust indicator, a rescaled
0–1 score, and the harmonised indicator, with the assumptions of each stated
explicitly.

## Design

- **Pooled two-wave design**, survey weights normalised within year so the
  waves carry equal weight.
- **Nested linear probability models**: demographics → socio-economic status
  → attitudes and institutional contact.
- **Heterogeneity**: cohort × wave interaction to identify who moved most.
- Standard errors clustered at the prefecture-city level.
- Analysis first written in Stata, then re-implemented in Python
  (`CGSS_judicial_trust_workflow.ipynb`) so the workflow is reproducible and
  the figures can be regenerated.

## Files in this folder

| File | Description |
|:--|:--|
| `CGSS_judicial_trust_workflow.ipynb` | Working notebook (harmonisation + descriptive results) |
| `CGSS2017_2023_pooled_python.csv` | Pooled two-wave dataset |
| `CGSS2017_cleaned_reference.csv` | Cleaned 2017 wave |
| `CGSS2023_cleaned_python.csv` | Cleaned 2023 wave |

## Note on scope

This folder documents the *design* of the study. The written proposal was
submitted through the course site. Detailed results and the manuscript are
being prepared separately and are not published here.

## Collaboration

| Member | Role |
|:--|:--|
| WANG Weicheng | Project coordinator and scribe — data acquisition, Stata cleaning and modelling, proposal and report writing |
| LI Siwei | Technical lead and progress tracker — `.dta` → `.csv` conversion, Python re-implementation, visualisations |
