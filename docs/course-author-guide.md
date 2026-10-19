---
title: Course Author Guide
intro: Organize community courses into clear learning paths, with useful practice and honest progress expectations.
description: How to structure FreeCampus Community Courses into journeys, courses, milestones, units, and lessons, with ungraded practice and browser-local progress.
---

This guide is for authors of **FreeCampus Community Courses**, the freely accessible public learning materials. Community authoring is unpaid volunteer work. Read the [Community Guide](community-guide.md) for contribution steps, licensing, credit, and the separate relationship with the App.

## Choose the learning structure

### Journey

A **journey is a group of courses**. When a community repository contains more than one course, call that collection a journey. A repository containing a single course can present it as a standalone course.

Give the journey a clear purpose and list its courses, their prerequisites, and a suggested order. Each course should still explain its own audience and learning outcomes.

### Course

A **course** develops a defined set of skills through units and lessons. It can organize its units into **milestones** when larger stages help learners understand the path. Milestones are optional; a course can also contain units directly.

### Milestone

A **milestone** contains units and a **milestone challenge**. Use the challenge to bring together what learners practiced across that milestone's units. Explain the outcome learners are working toward and how the units prepare them for it.

### Unit

A **unit** groups related lessons around a focused topic or outcome. It can also include a **unit challenge** to combine what learners practiced in those lessons. Unit challenges are optional.

### Lesson

A **lesson** introduces and practices a manageable part of a topic. Lessons usually do not have a dedicated challenge. Instead, check understanding through short quizzes, puzzles, worked examples, reflection questions, interactive exercises, or Google Colab notebooks where appropriate.

Choose activities that fit the subject and explain what learners should notice, try, or understand. Not every lesson needs every activity type.

## Example outline

This is an illustrative structure, not a required repository folder layout:

**Journey: Python** groups two courses: **Python Foundations** and **Python Automation**. The Foundations course could include this milestone:

- **Milestone: Work with everyday data**
    - **Unit: Values and variables**
        - Lesson: Explore values, with a prediction puzzle.
        - Lesson: Use variables, with a Google Colab exercise.
        - Optional unit challenge: Create a simple expense summary.
    - **Unit: Collections**
        - Lesson: Work with lists, with short understanding checks.
        - Lesson: Use dictionaries, with guided practice.
    - **Milestone challenge:** Combine variables and collections to summarize a small dataset.

The Automation course has its own units and lessons, with milestones where useful.

Follow the repository's existing file conventions. Discuss structural changes with maintainers before reorganizing published content or changing lesson URLs.

## Design practice without grades

**Community courses are not graded.** Lesson activities, unit challenges, and milestone challenges help learners practice and check their own understanding; they are not graded examinations.

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
- Use journey, course, milestone, unit, and lesson consistently. Include a milestone challenge wherever you introduce a milestone.
- Check that activities have useful feedback and that code, notebook links, and supporting files work.
- State the ungraded nature of the course and the limits of browser-local progress.
- Preserve required licenses and contributor credit, and follow the repository's review and build instructions.

[Discuss a course idea ↗](https://github.com/freecampus/freecampus.github.io/issues/new?title=Community%20course%20proposal){ .inline-action }
