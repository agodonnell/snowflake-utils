# Snowflake Utilities

A collection of reusable scripts, queries, and tools for working with the Snowflake data platform. This repository includes SQL scripts, Python utilities, and general workflow documentation for managing data pipelines, automation, and platform setup.

## 📁 Repository Structure

```
snowflake-utils/
├── sql/             # Raw SQL scripts for warehouse, roles, UDFs, views
├── scripts/         # Python or SnowSQL scripts for automation
├── notebooks/       # Optional: Jupyter notebooks for walkthroughs or demos
├── docs/            # Markdown documentation on workflows, tips, and setup
└── .github/workflows/ # CI/CD templates or GitHub Actions
```

## 🛆 Setup & Requirements

Some scripts assume the following are installed:

* Python 3.8+
* [SnowSQL CLI](https://docs.snowflake.com/en/user-guide/snowsql-install-config)
* `snowflake-connector-python` package

Install Python dependencies:

```bash
pip install -r requirements.txt
```

(Optional: Include `requirements.txt` if using Python)

## 🚀 Usage Examples

Run a Python script to refresh a materialized view:

```bash
python scripts/refresh_mat_view.py --env dev
```

Execute SQL to create a warehouse:

```bash
snowsql -f sql/warehouse_setup.sql
```

## 🧰 Scripts Overview

| File/Folder                      | Description                                      |
| -------------------------------- | ------------------------------------------------ |
| `sql/warehouse_setup.sql`        | Creates compute warehouses with scaling policies |
| `sql/udf_create_functions.sql`   | Defines Snowflake UDFs (e.g., masking, hashing)  |
| `scripts/refresh_mat_view.py`    | Refreshes a mat view programmatically            |
| `docs/snowflake_architecture.md` | Notes and diagrams on architecture decisions     |

## 😋 About

Created and maintained by [agodonnell.com](https://agodonnell.com).
For questions or suggestions, feel free to open an issue or contribute via PR.

## ❗ Licensing & Usage

All content in this repository — including code, scripts, images, documentation, and other assets — is copyright © 2025 AG ODonnell.
All rights are reserved.

This repository is intended solely for personal reference and portfolio purposes.
No content may be copied, reproduced, distributed, or used in any form without prior written permission from the copyright holder.
