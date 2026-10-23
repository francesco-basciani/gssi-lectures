# Software Architecture Description - Jupyter Book

Interactive teaching material for the GSSI **Software Architecture Description** course.

## Local preview

The project uses Jupyter Book 2 / MyST.

### Option A - Jupyter Book

```bash
python -m venv .venv
source .venv/bin/activate
pip install "jupyter-book>=2.1,<3"
jupyter book start
```

### Option B - MyST CLI

If `mystmd` is installed through npm:

```bash
myst start
```

The first preview may download the `book-theme` template.

## Static build

```bash
myst build --html
```

The static website is generated in:

```text
_build/html/
```

## GitHub Pages

A workflow template is provided in `deployment/github-pages.yml`.

Because GitHub Actions workflows must live at the **repository root**, copy it to:

```text
.github/workflows/deploy-software-architecture-description.yml
```

The template builds this project from:

```text
immigration-courses/software-architecture-description/
```

Then enable **Settings -> Pages -> Source: GitHub Actions** in the repository.

## Classroom use

The book is designed primarily for instructor projection. Students can optionally open the same website, but the main group exercise remains paper/whiteboard based.
