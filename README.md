# QA Toolkit

Free, fill-in-the-blank templates and checklists for manual QA testing of websites. Copy them into your own project, run your tests, and keep a clear record of what you checked, what failed, and what got fixed.

It is aimed at people learning manual QA, freelancers, and small teams who need a simple, repeatable process without a test management tool.

## What's Included

| Folder | File | Use it to |
|---|---|---|
| [Templates](Templates/) | [Test-Plan.md](Templates/Test-Plan.md) | Decide what to test, what to skip, and when testing is done |
| | [Test-Case.md](Templates/Test-Case.md) | Write step-by-step checks with expected results |
| | [Test-Execution-Log.md](Templates/Test-Execution-Log.md) | Record what happened each time a check was run |
| | [Bug-Report.md](Templates/Bug-Report.md) | Describe a bug so someone else can reproduce it |
| | [Test-Summary-Report.md](Templates/Test-Summary-Report.md) | Total the results and give a ready / not ready call |
| [Checklists](Checklists/) | [Website-Smoke-Test.md](Checklists/Website-Smoke-Test.md) | Quick check after a deployment or small change |
| | [Website-Regression-Test.md](Checklists/Website-Regression-Test.md) | Full check after a redesign or update, including accessibility |
| [Reference](Reference/) | [Testing-Types.md](Reference/Testing-Types.md) | Choose testing types and design techniques |
| | [Severity-vs-Priority.md](Reference/Severity-vs-Priority.md) | Rate how bad a bug is and how soon to fix it |
| | [Bug-Report-Examples.md](Reference/Bug-Report-Examples.md) | Compare a weak and a strong bug report |

Everything is plain Markdown. It renders on GitHub and opens in any text editor.

## Quick Start

**1. Get a copy.** Choose one:

- Select **Use this template** at the top of this page to create your own repository.
- Clone it: `git clone https://github.com/PaulMatasovsky/qa-toolkit.git`
- Select **Code > Download ZIP**.

**2. Create a folder for one test cycle** in the project you are testing, and copy in the files you need:

```bash
mkdir -p my-project/qa/2026-01-homepage-redesign/bugs
cp qa-toolkit/Templates/*.md my-project/qa/2026-01-homepage-redesign/
cp qa-toolkit/Checklists/Website-Smoke-Test.md my-project/qa/2026-01-homepage-redesign/
```

On Windows, copy the files in File Explorer instead.

**3. Follow the workflow below.** Delete the instruction lines (the ones starting with `>`) as you fill in each file.

A finished test cycle folder looks like this:

```text
qa/2026-01-homepage-redesign/
├── Test-Plan.md
├── Test-Case.md
├── Website-Smoke-Test.md
├── Test-Execution-Log.md
├── bugs/
│   ├── BUG-001.md
│   └── BUG-002.md
└── Test-Summary-Report.md
```

Keep the toolkit itself blank. Your results belong in your project, not in your copy of the toolkit.

## Workflow

1. **Plan.** Fill in the test plan: scope, browsers, and exit criteria.
2. **Prepare.** Pick a checklist, and write test cases for anything the checklist does not cover.
3. **Run.** Work through the checks and record every result in the execution log.
4. **Report.** For each failure, copy `Bug-Report.md` into `bugs/` as `BUG-001.md`, `BUG-002.md`, and so on. Add screenshots or recordings.
5. **Retest.** After a fix, run the failed check again and log it as a new row.
6. **Summarize.** Total the results in the summary report and give a recommendation.

For a small change, steps 1 and 2 can be as short as "run the smoke checklist."

## Rules for Safe Records

- Never write real passwords, personal data, or customer information in any file.
- Crop or blur screenshots that show private details before you share them.
- Mark a check as **Pass** only after you have run it.

## AI Transparency

I set the goals, scope, and structure of this toolkit. AI drafted the templates, checklists, and reference notes, and helped revise them. Review each file and adapt it to your project before you rely on it.

## Contributing

Suggestions are welcome. Open an issue describing the change and why it helps.

## License

[MIT](LICENSE). You can use, copy, and change these files for any purpose, including commercial work.
