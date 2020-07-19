# pre-commit for pytype

Wrapper to enable pre-commit for pytypes

## Usage:

In your `.pre-commit-config.yaml` include the following block.

```yaml
-   repo: https://github.com/sniperwolf/pre-commit-pytype
    rev: '2020.7.14'
    hooks:
    -   id: pytype
```

If you use `setup.cfg` instead of `-config=pytype.cfg` to run pytype then you will also need to include a empty args attribute in the pytype hook (exmple below).

```yaml
-   repo: https://github.com/sniperwolf/pre-commit-pytype
    rev: '2020.7.14'
    hooks:
    -   id: pytype
        args: []
```
