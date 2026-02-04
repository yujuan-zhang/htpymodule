# htpymodule-demo (with GitHub Actions)

Minimal Python package to practice:
- pytest tests in `tests/`
- GitHub Actions workflow in `.github/workflows/`

## Local test
```bash
python -m pip install -U pip
python -m pip install -e ".[test]"
python -m pytest -q
```

## GitHub Actions
Push to GitHub; Actions will run tests automatically on push/PR.
