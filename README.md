# Evidence Locker

Evidence Locker is a self-contained Federal Rules of Evidence study trainer. It turns evidence analysis into a case-file style practice desk with hypos, decision trees, flashcards, and progress tracking.

## Run It

No build step or dependencies are required. Open [Evidence Locker.html](Evidence%20Locker.html) directly in a modern browser.

For a local server, run:

```bash
python3 -m http.server
```

Then visit `http://localhost:8000/Evidence%20Locker.html`.

## Study Areas

The trainer covers:

- Relevance and Rule 403 balancing
- Character evidence
- Impeachment
- Privileges
- Lay and expert opinion
- Hearsay and the Confrontation Clause
- Authentication
- The Best Evidence Rule

## Main Views

### The Desk

The dashboard shows your rank, points, streak, topic accuracy, weakest area, and recommended next exercises. Progress is grouped by topic and tracked across both hypotheticals and journey maps.

### Practice Hypos

Work through evidence problems at four levels:

1. Rookie: single-issue problems
2. Associate: harder single-rule problems
3. Trial-Ready: multi-issue problems
4. Exam-Ready: mixed problems with a 1.5x point multiplier

Depending on the problem, you can cite the controlling rule, choose among answer options, write a short analysis, request a hint, and open explanations for each answer. Written answers can be self-graded or graded through the optional Claude sample capability when the host environment provides it.

### Journey Maps

Follow or construct an evidence decision path for:

- Hearsay and Confrontation
- Character Evidence
- Impeachment
- Privileges
- Lay and Expert Opinion
- Exhibits, Authentication, and the Best Evidence Rule

Click-through mode gives immediate route feedback. Build mode lets you arrange decision blocks, choose each branch, and compare your conclusion with the correct path.

### Quick Review

Use topic-filtered flashcards for rule numbers and key language, or run a 60-second rule-number sprint. Cards can be shown as rule numbers or language first.

## Progress and Privacy

Progress is saved locally in the browser under the `evidence-locker-v1` storage key. The app does not require an account or backend. Use the reset control on the desk to erase saved progress for the current browser.

The optional writing grader is only available when the surrounding host exposes `window.claude.use("sample")`; otherwise, written answers can be graded manually in the app.

## Project Files

- [Evidence Locker.html](Evidence%20Locker.html): complete application, including styles, study content, rule explanations, and client-side logic
- [README.md](README.md): project overview and usage instructions
