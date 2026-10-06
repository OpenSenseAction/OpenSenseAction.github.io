# OpenSense Software Overview Page

Documentation and examples for the OpenSense software ecosystem. The documentation site is available at [OpenSenseAction.github.io](https://OpenSenseAction.github.io).

## Repository structure

- `intro/` – introduction
- `software-ecosystem/` – notebooks for the main packages (poligrain, pycomlink, pypwsqc, mergeplg)
- `real_world_usage_examples.md` – real-world usage examples and method intercomparisons
- `training-schools.md` – workshop and training materials
- `related-software.md` – related packages (pyNNCML, RainfallQC, legacy packages)

## Build the docs locally

```bash
mamba env create -f environment.yml
mamba activate opensense-software
npm install -g mystmd
myst build .
```

## Run the examples locally

The example notebooks in `software-ecosystem/` can be run interactively in JupyterLab:

```bash
mamba activate opensense-software
jupyter lab
```

## License

BSD-3-Clause. See the [LICENSE](LICENSE) file.
