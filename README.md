# Lab 1 — Developer Environment

## Project description

This project is a starter application for CSC10014 Lab 1. It answers basic questions about university IT services.

## Prerequisites

- Python 3.10 or later
- Git
- VS Code (recommended)

## Setup

Clone the repository and enter the project directory:

```bash
git clone git@github.com:thanhhuong107/lab01-thanhhuong107.git
cd lab01-thanhhuong107
```

Create and activate a virtual environment on macOS/Linux:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install -e .
```

For Windows PowerShell, activate the environment with:

```powershell
py -m venv .venv
.venv\Scripts\Activate.ps1
```

Then install the dependencies using the same `pip` commands above.

## Run the application

```bash
python -m assistant "where is the IT helpdesk?"
```

Expected output:

```text
IT Helpdesk: room E.005, open Mon-Fri 08:00-17:00.
```

## Run tests

```bash
pytest -q
```

Expected result: all tests pass.

## Check the environment

```bash
python scripts/check_env.py
```

Expected result: all environment checks pass.

## Project structure

- `src/`: application source code
- `tests/`: automated tests
- `scripts/`: development and environment-check scripts
- `data/`: project data
- `docs/`: project documentation
- `ui/`: user interface resources
- `requirements.txt`: Python dependencies
- `pyproject.toml`: Python project configuration

## Troubleshooting

- If `pytest` is not found, activate `.venv` and reinstall `requirements.txt`.
- If imports fail, run `python -m pip install -e .`.
- If the environment check fails, read the reported problem and follow the relevant setup instructions.

## AI use

AI assistance may be used to understand errors and improve documentation. All generated changes should be reviewed, tested, and understood before committing.

## Virtual environment troubleshooting

If the virtual environment is not active, run:

```bash
source .venv/bin/activate
```

If dependencies are missing, run:

```bash
python -m pip install -r requirements.txt
python -m pip install -e .
```

Run `python scripts/check_env.py` to verify the setup.