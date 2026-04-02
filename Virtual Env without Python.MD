# Virtual Environments (Without Conda, Using Python's `venv`)

## 📂 Clean Folder Structure
This keeps environments organized and avoids cluttering system directories.
- PC - Users - User - Virtualenvs
C:\Users\TKH\virtualenvs

## ⚙️ Create Environment
- `py -m venv venv` → Create a new environment named `venv`
- `dir` (Windows) or `ls` (Linux/macOS) → Check the list of files/folders created

## ▶️ Activate Environment
- `py activate venv` → Create a new environment named `venv`

## ⏹ Deactivate Environment
- `deactivate` → Exit the environment

## ⏹ Remove Environment
- Remove-Item -Recurse -Force .\venv → Remove an environment named `venv`

## 📌 Additional Useful Points
- **Naming convention:** Use descriptive names, e.g. `venv_projectA`, `venv_projectB`
- **Requirements file:** Save dependencies with pip freeze > requirements.txt
- **Install Requirements:** pip install -r requirements.txt