# Getting Started

1. **Clone this repository:**
   ```bash
   git clone https://github.com/forgineer/demo-dbt.git
   cd demo-dbt
   ```

2. **Set up your environment and install dependencies using [uv](https://github.com/astral-sh/uv):**  
   `uv` is the preferred tool for managing this project.  
   Make sure `uv` is installed:
   ```bash
   pip install uv
   ```
   Then, run:
   ```bash
   uv sync
   ```
   This command will automatically create a virtual environment (if one does not exist) and install all dependencies as specified in `pyproject.toml`.

3. **Initialize dbt (if not already done):**
   ```bash
   dbt init dbt_duckdb
   ```
   **Sample output:**
   ```
   Running with dbt=1.10.13
   A project called dbt_duckdb already exists here.
   ```

4. **Run dbt debug to verify setup:**
   ```bash
   cd dbt_duckdb
   dbt debug
   ```
   **Sample output:**
   ```
   Running with dbt=1.10.13
   dbt version: 1.10.13
   python version: 3.12.12
   python path: /home/blake/Documents/demo-dbt/.venv/bin/python
   os info: Linux-6.12.48+deb13-amd64-x86_64-with-glibc2.41
   Using profiles dir at /home/blake/Documents/demo-dbt/dbt_duckdb
   Using profiles.yml file at /home/blake/Documents/demo-dbt/dbt_duckdb/profiles.yml
   Using dbt_project.yml file at /home/blake/Documents/demo-dbt/dbt_duckdb/dbt_project.yml
   adapter type: duckdb
   adapter version: 1.9.6
   Configuration:
     profiles.yml file [OK found and valid]
     dbt_project.yml file [OK found and valid]
   Required dependencies:
    - git [OK found]

   Connection:
     database: dev
     schema: main
     path: dev.duckdb
     config_options: None
     extensions: None
     settings: {}
     external_root: .
     use_credential_provider: None
     attach: None
     filesystems: None
     remote: None
     plugins: None
     disable_transactions: False
   Registered adapter: duckdb=1.9.6
     Connection test: [OK connection ok]

   All checks passed!
   ```