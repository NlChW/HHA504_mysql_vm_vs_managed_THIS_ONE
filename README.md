# HHA504_mysql_vm_vs_managed_THIS_ONE
# HHA504: MySQL on VM vs Managed Service (SQLAlchemy + pandas)

## Cloud chosen + region
- Cloud:
- Region:

## How to reproduce (high level)
1. Create VM and install/configure MySQL (port 22 + 3306 with IP restrictions).
2. Create a Managed MySQL instance and allowlist your IP.
3. Copy `.env.example` to `.env` and fill in connection values (do not commit `.env`).
4. Create Python venv and install dependencies.
5. Run:
   - `python scripts/vm_demo.py`
   - `python scripts/managed_demo.py`
6. Review outputs (table printed + row counts).

## Connection URL patterns (no secrets)
- PyMySQL:
  - `mysql+pymysql://USER:PASS@HOST:PORT/DBNAME`

## Where I stored secrets
- Local `.env` file (ignored by `.gitignore`)

## Screenshots
- VM: `screenshots/vm/`
- Managed: `screenshots/managed/`

## Docs
- VM notes: `docs/setup_notes_vm.md`
- Managed notes: `docs/setup_notes_managed.md`
- Comparison: `docs/comparison.md`
