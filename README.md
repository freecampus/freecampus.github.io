# FreeCampus

The public website for [FreeCampus](https://freecampus.org), a community creating free, rigorous learning materials across programming, mathematics, science, and more.

The site is built with MkDocs and a lightweight custom theme. All content lives in `docs/`, while the shared layout and visual system live in `theme/` and `docs/assets/`.

## Run locally

Create the project environment, then start the Makim preview task:

```bash
conda env create -f conda.yaml
conda activate freecampus
makim pages.preview
```

Open <http://127.0.0.1:8000>. For a production build, run:

```bash
makim pages.build
```
