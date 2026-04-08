# LLMOps — course materials

This repository holds **code alongs** (notebooks and small assets) for **MLOps / LLMOps and cloud platforms**, part of the **MLOps Engineer** programme at **Yrkeshögskolan**. The course runs over **six weeks**; new material is added under `code_alongs/` as the weeks go on.

## What’s in the repo

| Path | Purpose |
|------|--------|
| `code_alongs/` | Lecture notebooks, sample data, and related files per session |
| `pyproject.toml` / `uv.lock` | Python project metadata and locked dependencies |
| `.env.example` | Template for environment variables (API keys) |

## Prerequisites

- **Python 3.13** (see `.python-version`)
- **[uv](https://docs.astral.sh/uv/)** for installing dependencies and running Python

## Setup

1. Clone the repository and enter the project root.

2. Install dependencies:

   ```bash
   uv sync
   ```

3. Copy `.env.example` to `.env` and set your API key:

   ```bash
   cp .env.example .env
   ```

   The notebooks expect **`OPENROUTER_API_KEY`** for OpenRouter.

## Main dependencies

- `pydantic-ai` — agents and structured LLM workflows  
- `pandas` — tabular data where used in exercises  
- `ipykernel` — Jupyter kernel support  

Exact versions are pinned in `uv.lock`.
