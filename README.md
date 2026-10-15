# machine-learning-zoompcamp

## GitHub Codespaces

New Codespaces install Pipenv and sync the dependencies from `Pipfile.lock`
into a project virtual environment in `.venv`. VS Code uses that environment
for Python and notebooks. The virtual environment is intentionally not
committed; `Pipfile` and `Pipfile.lock` let a newly created Codespace recreate
it. `requirements.txt` is no longer used by Codespaces.

To add a package and record it for future Codespaces, run:

```bash
PIPENV_VENV_IN_PROJECT=1 python -m pipenv install package-name
```

Commit the updated `Pipfile` and `Pipfile.lock` along with your code.
