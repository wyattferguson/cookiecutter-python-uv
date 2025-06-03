---
title: Contributing
---

# Contributing Guidelines

## Issues

Only report issues for **{{cookiecutter.project_name}}**.

Before reporting an issue, please see if a similar issue is already open.
If applicable, also check if a similar issue has recently been closed
— your bug might have been just fixed.

To have your issue dealt with promptly, it's best to construct a
[minimal working example](https://en.wikipedia.org/wiki/Minimal_working_example) that exposes the issue in a clear and
reproducible manner.

## Installation

To install a developmental version of the project,
first [fork the project]. Then:

```
# spin up a virtual enviroment
uv venv

# activate virtual enviroment
.venv\Scripts\activate

# install all the cool dependancies
uv sync

# use taskipy to simplify running everything
task run
```

## Formatting & Testing

Please write reasonable unit tests for any new / changed functionality.
See [/tests/] directory for existing tests.
Before submitting a PR, ensure the tests pass:

```
task tests
```

Keep coding styling consistent by running:

```
# mypy typechecking
task typecheck

# ruff linting & typechecking combined
task lint

# format with ruff
task format
```

## Pull requests

If you're new to proposing changes on GitHub, help yourself to an
[appropriate guide](https://gist.github.com/Chaser324/ce0505fbed06b947d962). Additionally, please use explicit commit messages.
See [NumPy's development workflow](https://numpy.org/doc/stable/dev/development_workflow.html) for inspiration.
