---
title: Course Author Guide
intro: Organize community courses into clear learning paths, with useful practice and honest progress expectations.
description: How to structure FreeCampus Community Courses into journeys, courses, milestones, units, and lessons, with ungraded practice and browser-local progress.
---

This guide is for authors of **FreeCampus Community Courses**, the freely accessible public learning materials. Community authoring is unpaid volunteer work. Read the [Community Guide](community-guide.md) for contribution steps, licensing, credit, and the separate relationship with the App.

Use the [Lesson Editorial Guidelines](lesson-editorial-guidelines.md) to write individual lessons and review them before submission.

## Choose the learning structure

### Journey

A **FreeCampus Learning Journey**, or **Journey** for short, groups two or more related courses in the same community repository. A repository with one course can present it as a standalone course.

A **learning path** is a suggested route through a Journey. For example, the Python Journey starts with Python Foundations and offers paths into software development and scientific computing. See the [FreeCampus Python repository](https://github.com/freecampus/python).

When a large course would be easier to follow in smaller parts, split it into focused courses and keep them together as a Journey. Give each course its own audience and learning outcomes. On the Journey page, show where to start, what each course requires, and what learners can take next.

Reserve **program** for offerings with formal enrollment or completion requirements.

### Course

A **course** develops a defined set of skills and must be organized into one or more **milestones**. Each milestone contains units, and each unit contains lessons.

### Milestone

A **milestone** contains one or more units and must include a **milestone challenge**. Use the challenge to bring together what learners practiced across that milestone's units. Explain the outcome learners are working toward and how the units prepare them for it.

### Unit

A **unit** groups related lessons around a focused topic or outcome. Every unit must include a **unit challenge** to combine what learners practiced in those lessons.

### Lesson

A **lesson** introduces and practices a manageable part of a topic. Lessons usually do not have a dedicated challenge. Instead, check understanding through short quizzes, puzzles, worked examples, reflection questions, interactive exercises, or Google Colab notebooks where appropriate.

Choose activities that fit the subject and explain what learners should notice, try, or understand. Not every lesson needs every activity type.

## Write course content in Quarto

Write all course content in Quarto (`.qmd`). For lessons configured for Colab, the publishing pipeline generates a Jupyter notebook (`.ipynb`) from the lesson source and renders an **Open this lesson in Google Colab** link on the lesson page.

Follow the course repository’s conventions for notebook metadata and the shared Colab link. Make edits in the `.qmd` source so the published page and notebook reflect the same lesson. The [first Python Foundations lesson](https://github.com/freecampus/python/blob/main/docs/courses/python-foundations/milestones/first-programs/units/get-started/meet-python-first-program.qmd) shows the notebook metadata and link include in context.

## Example outline

This is an illustrative structure, not a required repository folder layout:

**Journey: Practical Programming** groups two courses: **Programming Foundations** and **Data Automation**. The Foundations course includes this milestone:

- **Milestone: Work with everyday data**
    - **Unit: Values and variables**
        - Lesson: Explore values, with a prediction puzzle.
        - Lesson: Use variables, with a Google Colab exercise.
        - Unit challenge: Create a simple expense summary.
    - **Unit: Collections**
        - Lesson: Work with lists, with short understanding checks.
        - Lesson: Use dictionaries, with guided practice.
        - Unit challenge: Organize a small inventory using lists and dictionaries.
    - **Milestone challenge:** Combine variables and collections to summarize a small dataset.

The Automation course follows the same required structure: milestones with milestone challenges, and units with lessons and unit challenges.

Follow the repository's existing file conventions. Discuss structural changes with maintainers before reorganizing published content or changing lesson URLs.

## Design practice without grades

**Community courses are not graded.** Lesson activities, unit challenges, and milestone challenges help learners practice and check their own understanding; they are not graded examinations.

Milestone and unit challenges are required parts of the course structure and remain ungraded.

For each activity or challenge:

- State the goal and provide clear instructions, prerequisites, and any starter files or data.
- Include useful feedback, hints, expected behavior, explanations, or a suggested solution so learners can review their work.
- Use quizzes or automated checks for learning feedback, without turning their results into a course grade or a pass requirement.
- Make activities readable on a phone and identify work that needs a computer or an external tool such as Google Colab.

Progress indicators show where a learner has reached. They are not grades or verified evidence of mastery. Do not promise instructor grading or individual review as part of a community course.

## Explain browser-local progress

Community course progress is stored locally in the learner's web browser. It is limited to the **same browser and browser profile on the same device**; it does not automatically synchronize to another device or browser.

Clearing the site's browser data can remove saved progress. Private browsing may discard it when the session ends. Do not describe this tracking as a cloud backup or imply that signing into the separate App restores community-course progress.

Include a short explanation near the course introduction or progress controls, for example:

> This course is ungraded. Your progress is saved in this browser on this device. It does not sync across devices and may be lost if you clear the site's browser data.

These progress and grading rules describe Community Courses. The separate App has its own product design and implementation.

## Before submitting

- Explain the audience, prerequisites, learning outcomes, and suggested learning order.
- Use journey, course, milestone, unit, and lesson consistently. Organize every course into milestones and include a milestone challenge in each milestone.
- Include lessons and a unit challenge in every unit.
- Check that activities have useful feedback and that code, notebook links, and supporting files work.
- State the ungraded nature of the course and the limits of browser-local progress.
- Preserve required licenses and contributor credit, and follow the repository's review and build instructions.

[Discuss a course idea ↗](https://github.com/freecampus/freecampus.github.io/issues/new?title=Community%20course%20proposal){ .inline-action }
