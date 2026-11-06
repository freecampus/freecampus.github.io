---
title: Lesson Editorial Guidelines
intro: Write lessons with clear goals, useful examples, and feedback learners can use on their own.
description: Editorial guidance and a review checklist for authors of FreeCampus Community Course lessons.
---

Use these guidelines to write and review lessons for FreeCampus Community Courses. The [Course Author Guide](course-author-guide.md) explains how lessons fit into units and milestones and how ungraded practice works.

## Plan the lesson

- **Give the lesson one main outcome.** Say what learners will be able to do, using a verb such as explain, compare, calculate, configure, or debug. “Distinguish correlation from causation in a news claim” gives learners a concrete target.
- **Explain why the outcome matters.** A short case, question, or use case can show where the idea applies before you introduce the details.
- **State prerequisites and access needs up front.** Link to earlier lessons where possible. Say when learners need a computer, a particular operating system, an account, a download, or physical materials.

### Put examples and practice close to the explanation

1. **Introduce the idea.** Explain one meaningful idea at a time. Use headings that describe what the learner will do or understand.
2. **Show how it works.** Place a worked example, case, diagram, or demonstration beside the idea it illustrates. Explain the decisions behind it.
3. **Let learners try.** Ask them to apply or explain what they learned. Say what to produce and provide feedback they can use on their own, such as a hint, a worked answer, an expected result, or criteria for a well-reasoned response.

Repeat this sequence after a meaningful step. A short concept lesson may need one cycle, and a multi-step workflow may need several. Close with a brief recap or a link to the next lesson or challenge when it helps learners continue.

## Write for a global, mobile-first audience

- Address the learner directly. Use plain, precise language, short paragraphs, descriptive headings, and numbered steps for procedures. Explain steps that words such as “obviously” or “just” would gloss over.
- Define unfamiliar terms, acronyms, and symbols when they first matter. Use consistent terminology in explanations, exercises, and feedback. Match interface labels and code identifiers exactly.
- Give examples that make sense across regions or explain the local context. Include the units, date formats, and currency learners need to interpret the example.
- Use images, diagrams, and screenshots where they clarify an idea or action. Provide useful alt text for informative images and explain complex visuals in nearby text. Use readable labels and contrast. Identify items by name or position as well as color. Keep commands, code, formulas, and essential instructions available as text. Emojis are optional and should carry no essential meaning on their own.
- Preview the lesson on a narrow screen. Keep media and downloads small where practical. If an activity requires a computer or a large download, keep the explanation and expected result readable on a phone.
- Cite sources for quotations, data, and claims that need evidence. Record the source, license, and required credit for reused images, code, and datasets. Label fictional or simplified examples when learners might otherwise read them as evidence.

## Choose the approach by what learners will do

These approaches can be combined. An engineering lesson might introduce a concept, work through a calculation, and use a simulation to check the result.

### Concepts, theory, and interpretation

Define the concept, distinguish it from a related idea, and show where it applies or where it breaks down. When interpretations differ, explain the scope of each view and what evidence supports it. A short prompt to compare, classify, predict, or explain can be enough practice. For open-ended questions, describe what a defensible answer includes and accept multiple well-reasoned answers.

For example, after introducing correlation and causation, ask learners to explain whether a study headline supports a causal claim and name one piece of evidence that would strengthen it.

### Calculation, quantitative reasoning, and proofs

State the givens, assumptions, notation, and units where applicable. Explain why each key step in a worked example follows. Show how to check the result using an estimate, a unit check, substitution, or a boundary case. Then change an input or condition and ask learners what changes. In a proof lesson, ask learners to identify where an assumption is used and what happens if it is dropped.

### Software and tool workflows

State the starting point, supported environment, and expected result. Use the actual menu labels, button names, and commands. Note relevant differences across Windows, macOS, and Linux. Use a cropped, readable screenshot when learners need to locate a control or recognize an output. Give the same essential directions in text.

For example, in a lesson about an integrated development environment (IDE), show how to select the Python interpreter, run a file, and verify which interpreter ran it. Include a recovery step if the IDE selects a different environment.

### Labs, fieldwork, and design

List materials, conditions, and relevant safety requirements. Explain what learners should measure, record, build, or decide. Provide a sample result or trade-off and show how to recognize a setup or measurement error. When practical, offer sample data or a lower-equipment option that supports the same reasoning.

### Programming

- **Teach a skill at a time.** Introduce the concept, its purpose, and a use case. Explain the library, function, method, class, or parameter when it becomes useful. Show relevant inputs, outputs, or side effects and why the example uses that tool. Link to documentation for details beyond the lesson.
- **Pair short explanations with runnable code.** Show the expected output or behavior. Give learners something to predict, run, trace, modify, or debug before moving to another substantial concept. State any setup the example depends on.
- **Use checkpoints to help learners recover.** After a meaningful intermediate step, explain what learners should see, why it looks that way, and what to inspect if their result differs. A checkpoint might show a table’s expected shape or a variable’s value before the next step.
- **Add short quizzes at meaningful transitions.** This is strongly recommended. Ask learners to predict an output, choose an explanation, or identify a likely bug. Explain the reasoning in the feedback, especially when a plausible wrong answer reveals a common misunderstanding.
- **Make practice a small step beyond the example.** Keep the target concept and change the dataset, condition, or input. Give a starting point and success criteria. Offer hints before a worked solution, then explain the solution so learners can compare it with their own approach.
- **Model readable, documented code.** Use meaningful names. For Python, include docstrings for functions, methods, and classes written for the lesson. Use the course’s chosen convention consistently. Explain relevant parameters, return values, exceptions, and side effects. PEP 257 gives general conventions, while Google and NumPy offer structured styles. If your course uses Douki’s YAML docstring format, include a short example. [PEP 257](https://peps.python.org/pep-0257/) · [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) · [NumPy docstring guide](https://numpydoc.readthedocs.io/en/latest/format.html) · [Douki](https://github.com/arxlang/douki)
- **Use assertions where they give useful feedback.** Check behavior and accept different implementations that meet the same requirements. Cover a representative case and a relevant edge case when applicable. Give failure messages that tell learners what to inspect. For exploratory or visual work, an expected observation may be a better check. These checks support self-review in community lessons.
- **Verify the learner’s execution path.** For Quarto lessons intended for Colab, write executable cells in the `.qmd` source, convert to `.ipynb`, and open the generated notebook in Colab. In a fresh runtime, run setup and examples in order and try the practice and feedback as a learner would. Make dependencies and data loading explicit. Verify local workflows in the environment the lesson specifies. [Quarto notebook conversion](https://quarto.org/docs/cli/convert.html)

#### Example of a programming lesson sequence

The goal is to filter a table by a numeric condition and explain which rows qualify.

1. **Explain and demonstrate.** Use a small rainfall table to select days with at least 10 mm of rain. Show the condition and filtered output next to the code.
2. **Check the boundary.** The result should include the day with exactly 10 mm. Explain that `>=` includes the boundary. If that row is missing, check the comparison operator.
3. **Quiz.** Ask which rows would change with `>`. The feedback explains why the day with exactly 10 mm would be excluded.
4. **Practice.** Use a small transit table with trips of 14, 15, and 16 minutes. Ask learners to keep trips of at most 15 minutes and explain which trip IDs the assertions should expect.

A later Unit Challenge can ask learners to load, clean, and filter a new table, with links to the lessons on each skill.

## Name activities consistently

- **Checkpoint** helps learners verify an intermediate result and recover if it differs.
- **Quiz** asks one or more short questions and explains the reasoning behind the answers.
- **Practice** applies the current lesson skill. Use **Lab** for practice with a dedicated notebook, workspace, or hands-on procedure.
- **Unit Challenge** combines skills taught in the unit.
- **Milestone Challenge** combines skills from the milestone’s units.

Use **project** for what learners build when a challenge has a project deliverable. A lesson can use a running example or a small lab to teach an individual skill. Place larger programming projects in Unit Challenges or Milestone Challenges, after the tools and concepts they depend on have been taught. Link each challenge to the relevant lessons so learners can revisit them.

## Review checklist

Mark each applicable criterion **Meets** or **Revise**. Use **N/A** for criteria outside the lesson’s scope. Resolve items marked **Revise** before approval. Keep suggestions about recommended practices separate. When requesting a revision, point to the section, explain the problem for the learner, and describe what would resolve it.

1. **Outcome and scope.** The lesson has an observable outcome, a clear purpose, and any necessary prerequisites or access requirements.
2. **Sequence.** Ideas build in a usable order, with examples or demonstrations close to the explanations they support.
3. **Practice and feedback.** Learners can attempt a check aligned with the outcome and understand why their result is sound or what to try if it differs.
4. **Language and access.** Terms are consistent, instructions and visuals are accessible, and the lesson is readable on a phone.
5. **Accuracy and attribution.** Claims, examples, expected results, and sources are accurate. Reused material includes the required license information and credit.
6. **Lesson approach.** The lesson provides the information its activity needs, such as model reasoning for an interpretation, units and assumptions for a calculation, or expected results and recovery steps for a software workflow.
7. **Programming.** Examples and practice checks work in the stated environment. Checkpoints help learners diagnose likely errors. Authored Python functions, methods, and classes follow the selected docstring convention.
8. **Challenge placement.** The lesson focuses on its own skills. Any related Unit Challenge or Milestone Challenge uses the correct label and links back to the lessons it draws on.

For a review pass, try the main activity before looking at the solution. Make one likely mistake and see whether the feedback helps you recover.
