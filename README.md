# FreeCampus

This repository contains the MkDocs site for [FreeCampus](https://freecampus.org/), a community that creates free learning materials across programming, mathematics, science, and other subjects.

## Explore and contribute

- [Subjects](https://freecampus.org/subjects/) — find courses and learning materials.
- [Contribute](https://freecampus.org/contribute/) — find ways to help and get started.
- [Community Guide](https://freecampus.org/community-guide/) — learn how contributions, licensing, and review work.
- [Course Author Guide](https://freecampus.org/course-author-guide/) — organize and publish community courses.
- [Lesson Editorial Guidelines](https://freecampus.org/lesson-editorial-guidelines/) — write and review individual lessons.

## Work on the site locally

Site content is in `docs/` and the MkDocs theme is in `theme/`.

From the repository root, create the Conda environment and start the preview.

```bash
conda env create -f conda.yaml
conda activate freecampus
makim pages.preview
```

Open <http://127.0.0.1:8000>. To generate the static site in `build/`, run the build task.

```bash
makim pages.build
```
