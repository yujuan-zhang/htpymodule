# htpymodule-demo (with GitHub Actions)

## What it does

Minimal Python package to practice:
- pytest tests in `tests/`
- GitHub Actions workflow in `.github/workflows/`

## Input

Input is an optional name string, and output is a returned greeting string; no CSV or generated file is needed.

## Output

Expected terminal output: `Hello, Yujuan!`.  `hello()` returns `Hello, world!`. Both examples were verified from the source package. The existing tests check these cases; installation and CI execution were not benchmarked.

## Try it

### First call

Requires Python >= 3.9. From this repository:

```bash
python -m pip install -e .
python -c 'from htpymodule import hello; print(hello("Yujuan"))'
```



### Local test

```bash
python -m pip install -U pip
python -m pip install -e ".[test]"
python -m pytest -q
```

### GitHub Actions

Push to GitHub; Actions will run tests automatically on push/PR.

