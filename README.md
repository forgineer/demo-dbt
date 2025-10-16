# dbt DuckDB Demo

## Purpose

This repository is a well-documented, minimal outline for using **dbt-core** as a data transformation tool.  
It is designed for data engineers who want a clear, step-by-step guide to dbt-core, without the complexity or ambiguity often found in official documentation.

## Why This Repo?

- The official dbt documentation can be difficult to follow, even for experienced engineers.
- This guide aims to be concise, practical, and easy to use.
- No sign-ups, cloud accounts, or risk of incurring charges—**DuckDB** is used as the data warehouse for its simplicity and local operation.

## dbt-core vs dbt-fusion

- **dbt-core**: The open-source, command-line tool for data transformation.  
  This repo focuses exclusively on dbt-core to keep things minimal and avoid external dependencies.
- **dbt-fusion**: Refers to dbt’s cloud-based, managed offering.  
  This repo does **not** cover dbt-fusion, so you won’t need to sign up for any services.

## How to Use This Repository

1. **Clone the repo and set up a Python virtual environment.**
2. **Install dependencies:**  
   - `dbt-core`  
   - `dbt-duckdb`
3. **Initialize your dbt project:**  
   - The project is pre-configured for DuckDB.
4. **Follow the documented steps and notes in each folder** to learn dbt concepts and workflows.
5. **No cloud accounts or paid services required.**  
   Everything runs locally using DuckDB.

## Getting Started

1. **Clone this repository:**
   ```bash
   git clone https://github.com/your-username/demo-dbt.git
   cd demo-dbt
   ```

2. **Create and activate a Python virtual environment:**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies using [uv](https://github.com/astral-sh/uv):**  
   Using `uv` helps ensure consistent Python versions and library resolution.
   ```bash
   pip install uv
   uv pip install -r requirements.txt
   ```
   Or, if using a `pyproject.toml`:
   ```bash
   uv pip install -r pyproject.toml
   ```

4. **Initialize dbt (if not already done):**
   ```bash
   dbt init dbt_duckdb
   ```

5. **Run dbt debug to verify setup:**
   ```bash
   cd dbt_duckdb
   dbt debug
   ```

## Next Steps

- Explore the README files in each subfolder for explanations of dbt concepts.
- Start transforming data using dbt models and seeds.
- Use this repo as a reference for your own dbt-core projects.

---

Feel free to contribute improvements or clarifications as you learn!
