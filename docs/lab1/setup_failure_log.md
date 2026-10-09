# Lab 1 — Setup Failure Log

## Failure 1: Virtual environment missing

**What I did:**  
I deleted the `.venv` directory to simulate a broken development environment.

**Symptom:**  
The project's virtual environment and its installed packages were no longer available.

**How I recovered:**  
I followed the setup instructions in `README.md`:
1. Created a new virtual environment with `python3 -m venv .venv`.
2. Activated it with `source .venv/bin/activate`.
3. Installed dependencies with `python -m pip install -r requirements.txt`.
4. Installed the project with `python -m pip install -e .`.
5. Ran the application and `pytest -q` to verify the setup.

**Verification:**  
Record the actual application output and pytest result here.

**README improvement:**  
I checked that the README explains how to recreate `.venv`, install dependencies, run the application, and run tests.