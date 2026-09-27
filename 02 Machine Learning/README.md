# 02 Machine Learning

**Status: existing study materials.** This stage contains the four workspaces
that previously sat at the repository root. Their notebook contents, datasets,
project files, and local setup instructions remain within their original
workspace folders.

| Workspace | Start here | Focus |
| --- | --- | --- |
| `Python For Machine Learning IBM` | [IBM guide](<Python For Machine Learning IBM/README.md>) | Regression, classification, clustering, validation, and local labs |
| `Machine Learning Andrew` | [Andrew guide](<Machine Learning Andrew/README.md>) | Supervised learning, advanced algorithms, unsupervised learning, recommenders, and reinforcement learning |
| `Machine Learning at RMIT` | [RMIT guide](<Machine Learning at RMIT/README.md>) | Weekly course notes, datasets, assignments, and notebooks |
| `Machine Learning tổng` | [Lifecycle handbook](<Machine Learning tổng/README.md>) | Problem framing through evaluation, deployment, monitoring, and retirement |

## Running a workspace

Change into the chosen Python workspace before running `uv sync --locked` or
opening Jupyter. Each workspace has its own `pyproject.toml`, `uv.lock`,
`.python-version`, and README; do not install all three as one project. Follow
the workspace guide for its Python version, kernel, separate TensorFlow
environment when needed, and notebook working directory.

The handbook is documentation only. After this stage, continue to
[03 Deep Learning](<../03 Deep Learning/README.md>).
