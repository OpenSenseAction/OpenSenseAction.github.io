# Contributing

Contributions to the OpenSense software ecosystem are very welcome! The packages follow a common development workflow, which is described in detail in the [poligrain contributing guide](https://poligrain.readthedocs.io/en/latest/development/CONTRIBUTING.html).

## Guidelines in brief

- Contributions should go through a pull request (PR), ideally linked to an open issue for discussing the implementation first.
- Code format and style are enforced by linting tools (`pre-commit`); run `pre-commit run -a` before committing.
- New code must have 100% test coverage (exceptions need to be discussed with the maintainers).

## Typical workflow

1. **Fork and clone** the repository you want to contribute to.
2. **Set up the dev environment**: create a `conda` environment (Python 3.10 or 3.11) and install `poetry`, `nox` and `pre-commit`, then run `poetry install`.
3. **Write code and commit**: activate the pre-commit hooks with `pre-commit install`, work on a feature branch, and commit regularly.
4. **Open a pull request**: sync your fork with the upstream repository, push your branch, and open a PR. The CI will run linting and tests, and test coverage is reported automatically.

## Running checks locally

- `nox -s lint` — linting
- `nox -s tests` — Python tests
- `nox -s docs -- --serve` — build and serve the docs locally

For the full step-by-step guide, including details on writing tests and troubleshooting, see the [complete contributing guide](https://poligrain.readthedocs.io/en/latest/development/CONTRIBUTING.html).
