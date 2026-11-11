# Undoing AI Agent Actions under Concurrent Human Edits

Research project by **W. T. Y. Kavinda** (Faculty of Computing, Sabaragamuwa University of Sri Lanka).

LLM agents (for example agents that call tools through the Model Context Protocol, MCP) change
shared documents, boards and files. When the user clicks "undo", people may have edited the same
state in the meantime, and a plain rollback can destroy their work. This project studies how
agent actions can be undone safely when humans edit at the same time.

This repository holds the whole project: the literature review, the implementation and the experiments.

## Repository layout

| Folder | Content | Status |
|---|---|---|
| `slr/` | Systematic literature review data: search log, screening decisions, coded data for the 175 included studies (`21CIS0136_SLR_workbook.xlsx`) | Available |
| `docs/` | Written outputs (SLR report, figures) | SLR report to be added |
| `implementation/` | Source code of the proposed undo approach and tools | Planned |
| `experiments/` | Experiment scripts, data and results | Planned |

## Part 1 - Systematic literature review

Title: *Undoing AI Agent Actions under Concurrent Human Edits: A Systematic Literature Review*.
It follows Kitchenham and Charters (2007) and PRISMA 2020.

1,483 database records and 58 other-source records were identified. After duplicate removal,
1,365 titles, 432 abstracts and 182 full reports were screened, and **175 studies were included**
(121 from databases, 54 from other sources). Searches cover records up to 9 November 2026.
Screening was done by one reviewer (see the Limitations section of the report).

Workbook sheets (`slr/21CIS0136_SLR_workbook.xlsx`):

- **Summary of the Study**: topic, objectives, research questions, methods, results summary.
- **Search Log**: search date, string, years, export format and records retained for every database.
- **IEEE Explorer, ACM Digital Library, SpringerLink, Science Direct, Compendex, Emerald, Sage, Wiley, Taylor & Francis, arXiv**: the records retrieved from each source.
- **Other sources & Snowballing**: records found by snowballing and other sources.
- **Screening & PRISMA**: every unique record with its decision, code (I1-I6 / E1-E7) and reason at each stage.
- **SLR Coding**: coded data and quality scores (Q1-Q6) for the included studies.

## How to cite

Use GitHub's **Cite this repository** button (it reads `CITATION.cff`).
To cite a fixed state of the repository, cite a tagged release, for example `v1.0.0`.

## Licence

- Data in `slr/`: CC BY 4.0 (<https://creativecommons.org/licenses/by/4.0/>). Reuse is allowed with credit to the author.
- Code: MIT (see `LICENSE`).
- Titles, abstracts and metadata of the reviewed papers belong to their authors and publishers and are included only to document the review. Full texts are not redistributed.
