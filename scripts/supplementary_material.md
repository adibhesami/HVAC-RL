name: Unit & Style

on: [push, pull_request]

jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-python@v5
        with:
          python-version: '3.10'
      - name: Install
        run: |
          pip install -r <(conda env export --from-history)
      - name: Black format check
        run: black --check scripts/*.py
