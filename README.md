# machine-learning-zoompcamp

## GitHub Codespaces

New Codespaces set up a project virtual environment in `.venv` and install the
packages listed in `requirements.txt`. VS Code uses that environment for Python
and notebooks. The virtual environment is intentionally not committed; the
requirements file lets a newly created Codespace recreate it.

Installing a package does not update `requirements.txt` automatically. After
each new install, refresh the file so the package and its installed
dependencies are available in future Codespaces:

```bash
.venv/bin/python -m pip install package-name
.venv/bin/python -m pip freeze > requirements.txt
```

Replace `package-name` with the package's pip name. Commit the updated
`requirements.txt` along with your code.