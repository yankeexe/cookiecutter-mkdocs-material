# {{cookiecutter.documentation_name}}


> Note: [MKDocs Documentation](https://squidfunk.github.io/mkdocs-material/getting-started/)


## Usage

### Virtual environment setup

Create a virtual environment.

```bash
$ make venv
```

Activate virtual environment.

```bash
$ source venv/bin/activate
```

### Setup Docs

Install depenedencies

```bash
$ make setup
```

Run the docs

```bash
$ make run
```

## Adding docs

Add documents to the designated folder for different entities. One can add different markdown files inside of the designated folder and have to add the navigation paths on `nav` section of the `mkdocs.yml` file.
