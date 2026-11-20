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

## Support & Acknowledgments

### Help keep quality learning open to everyone

FreeCampus Community Courses bring learners and educators together to create materials that anyone can read and improve. Clear explanations, practical activities, accessible pages, and thoughtful review all take time and care. We welcome educators, developers, translators, reviewers, and learners who want to make those resources more useful.

**[Contribute to FreeCampus](https://freecampus.org/contribute/)**. You can help by improving a lesson, reviewing an explanation, reporting an issue, or working on the open website and learning tools.

### Credits and thanks

[SciStitch](https://scistitch.com/) leads development and maintenance of the FreeCampus ecosystem, spanning Community Courses and the separate FreeCampus App. Open course materials are authored and improved by the FreeCampus community; the App has its own operating model. We thank [Open Science Labs (OSL)](https://opensciencelabs.org/) for institutional support, and every author, reviewer, translator, designer, developer, learner, and user who shares their knowledge and feedback.

<p>
  <a href="https://scistitch.com/"><img src="https://scistitch.com/images/logo/wordmark-color.svg" alt="SciStitch" width="160" style="background: #fff; border-radius: 6px; padding: 6px 8px;"></a>
  &nbsp;&nbsp;
  <a href="https://opensciencelabs.org/"><img src="https://scistitch.com/assets/osl-logo.svg" alt="Open Science Labs" width="128" style="background: #fff; border-radius: 6px; padding: 6px 8px;"></a>
</p>
