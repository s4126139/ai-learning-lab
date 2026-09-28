# AI Learning Lab

A study path from mathematics and classical machine learning to deep learning,
LLM applications, AI agents, and a capstone project. The numbered stage folders
are at the repository root. **Completed** marks prior study; **planned** stages
are a roadmap, not a claim that their exercises are finished.

| Stage | Focus | Status | Start here |
| --- | --- | --- | --- |
| 01 | Foundation Mathematics: MIT 18.01, 18.02, 18.05, 18.06 | Completed | [Foundation Mathematics](<01 Foundation Mathematics/README.md>) |
| 02 | Machine Learning: IBM, Andrew Ng, RMIT, and lifecycle handbook | Existing study materials | [Machine Learning](<02 Machine Learning/README.md>) |
| 03 | Deep Learning Specialization | Planned | [Deep Learning](<03 Deep Learning/README.md>) |
| 04 | PyTorch Learn the Basics | Planned | [PyTorch](<04 PyTorch/README.md>) |
| 05 | Stanford CS224N and LLM foundations | Planned | [NLP and LLM Foundations](<05 NLP and LLM Foundations/README.md>) |
| 06 | LLM Zoomcamp and application evaluation | Planned | [LLM Applications](<06 LLM Applications/README.md>) |
| 07 | Hugging Face Agents Course | Planned | [AI Agents](<07 AI Agents/README.md>) |
| 08 | Integrated capstone | Planned | [Capstone](<08 Capstone/README.md>) |

## RMIT Classical AI courses

The university courses follow their teaching periods alongside the numbered
self-study stages. [RMIT Classical AI](<RMIT Classical AI/README.md>) holds the
planned games and AI course for March 2027 and the general AI course for July
2027. They cover search, planning, uncertainty, and reinforcement learning;
stage 07 remains the Hugging Face Agents Course.

## Existing Machine Learning workspaces

The four original folders now live together under `02 Machine Learning`:

| Workspace | Contents | Guide |
| --- | --- | --- |
| IBM Machine Learning with Python | Concept notes and local labs | [IBM guide](<02 Machine Learning/Python For Machine Learning IBM/README.md>) |
| Andrew Ng Machine Learning Specialization | Three courses of notes, helpers, and labs | [Andrew guide](<02 Machine Learning/Machine Learning Andrew/README.md>) |
| RMIT Machine Learning | Week notes, teaching files, datasets, and notebooks | [RMIT guide](<02 Machine Learning/Machine Learning at RMIT/README.md>) |
| ML lifecycle handbook | Project design, evaluation, deployment, and monitoring guides | [Handbook](<02 Machine Learning/Machine Learning tổng/README.md>) |

Each of the three Python workspaces keeps its own `pyproject.toml`, `uv.lock`,
`.python-version`, and setup guide. Install [uv](https://docs.astral.sh/uv/),
change into the workspace you want, and run `uv sync --locked` there. Start
Jupyter from the notebook or lab directory as its guide describes so local
data paths and helper imports resolve. The pinned Python versions are 3.12 for
IBM, 3.14 for Andrew, and 3.14.5 for RMIT. Andrew Course 2 and 3 and RMIT
Week 8–9 TensorFlow labs use separate Python 3.12 environments described in
their guides.

Saved notebook code and outputs remain available for reading on GitHub. To
reproduce a result, use that workspace's environment, restart its kernel, and
run cells in order. Some RMIT notebooks are course templates or older copies
without a saved run.

## Data and access

- Most lab data is next to its notebook. The IBM fraud lab's 151 MB
  `creditcard.csv` is excluded from Git; follow the
  [fraud data instructions](<02 Machine Learning/Python For Machine Learning IBM/Module 3 Building Supervised Learning Models/labs/data/README.md>).
- RMIT Canvas pages require a course login. The
  [local material manifest](<02 Machine Learning/Machine Learning at RMIT/canvas_materials_manifest.md>)
  records captured material and unresolved slide placeholders. Two retained
  assignment brief PDFs still contain original course links.
- The RMIT ASM1 assignment and supplied dataset remain excluded because their
  use is restricted to the course. The separate [MLA2 project and demo](<02 Machine Learning/Machine Learning at RMIT/MLA2.md>)
  are linked from this repo, while its checkout remains outside this Git tree.
  In `ASM2-3`, group deliverables are excluded by `.gitignore`; assignment
  briefs and the personal HTML lab are included.

## Repository checks

Run `uv lock --check` inside each Python workspace to check its lockfile. A
fresh Jupyter installation can validate a notebook with
`python -m nbconvert --to notebook --execute <file.ipynb>`; training labs may
take time and need the datasets noted above. Keep credentials, local virtual
environments, and generated model files out of Git.
