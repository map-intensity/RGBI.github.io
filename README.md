# Documentation example

We use this example in one [CodeRefinery](https://coderefinery.org/) lesson:
- https://coderefinery.github.io/documentation/

## The Environment

The environment in which to run the notebooks and build the books is defined in
[environment.yaml]().
To recreate and activate the environment locally, run

```
conda env create -f environment.yaml
conda activate coderefinery

```

## Build
To build the book locally, you should first create and activate your environment,
as described above. Then run

```
sphinx-build doc _build
```

### Verify integrity
```
sphinx-build doc -W -b linkcheck -d _build/doctrees _build/html
```
