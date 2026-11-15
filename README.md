# QA Toolkit

**Project status:** **In Progress** · **Activity:** Active (templates ready; first use planned on my portfolio website)

Fill-in-the-blank templates and checklists for manual QA testing of websites. I built this so I could test my own site with a repeatable process, and I made it general so anyone can clone it and use it on theirs.

It suits people learning manual QA, freelancers, and small teams who want a clear record of what was tested, what failed, and what got fixed, without a paid test management tool.

## What's Included

| Folder | File | Use it to |
|---|---|---|
| [Templates](Templates/) | [Test-Plan.md](Templates/Test-Plan.md) | Decide what to test, what to skip, and when testing is done |
| | [Test-Case.md](Templates/Test-Case.md) | Write step-by-step checks with expected results |
| | [Exploratory-Session.md](Templates/Exploratory-Session.md) | Record a time-boxed, unscripted testing session |
| | [Test-Execution-Log.md](Templates/Test-Execution-Log.md) | Record test case runs and retests |
| | [Bug-Report.md](Templates/Bug-Report.md) | Describe a bug so someone else can reproduce it |
| | [Test-Summary-Report.md](Templates/Test-Summary-Report.md) | Total the results and give a ready / not ready call |
| [Checklists](Checklists/) | [Website-Smoke-Test.md](Checklists/Website-Smoke-Test.md) | Run 16 quick checks after a deployment or small change |
| | [Website-Regression-Test.md](Checklists/Website-Regression-Test.md) | Run 33 checks after a redesign or update, including accessibility and WordPress |
| [Reference](Reference/) | [Testing-Types.md](Reference/Testing-Types.md) | Choose testing types and test design techniques |
| | [Severity-vs-Priority.md](Reference/Severity-vs-Priority.md) | Rate how bad a bug is and how soon to fix it |
| | [Bug-Report-Examples.md](Reference/Bug-Report-Examples.md) | Compare a weak and a strong bug report |
| | [Free-Tools.md](Reference/Free-Tools.md) | Find free tools for links, accessibility, and performance |

Everything is plain Markdown. It reads well on GitHub and opens in any text editor.

## Quick Start

**1. Get a copy.** Choose one:

- Select **Use this template** at the top of this page to create your own repository.
- Clone it: `git clone https://github.com/PaulMatasovsky/qa-toolkit.git`
- Select **Code > Download ZIP**.

**2. Create a folder for one test cycle** in the project you are testing:

```bash
CYCLE=my-project/qa/2026-01-homepage-redesign
mkdir -p $CYCLE/bugs $CYCLE/evidence
cp qa-toolkit/Templates/Test-Plan.md qa-toolkit/Templates/Test-Execution-Log.md qa-toolkit/Templates/Test-Summary-Report.md $CYCLE/
cp qa-toolkit/Checklists/Website-Smoke-Test.md $CYCLE/
```

On Windows, create the folders and copy the files in File Explorer.

**3. Work through the [workflow](#workflow).** Delete the instruction lines (the ones starting with `>`) as you fill in each file.

A finished test cycle looks like this:

```text
qa/2026-01-homepage-redesign/
├── Test-Plan.md
├── Website-Smoke-Test.md
├── Test-Case.md               (optional)
├── Exploratory-Session.md     (optional)
├── Test-Execution-Log.md
├── Test-Summary-Report.md
├── bugs/
│   └── BUG-001.md
└── evidence/
    └── BUG-001-mobile-menu.png
```

Keep your copy of the toolkit blank. Results belong with the project being tested.

## Workflow

1. **Plan.** Fill in the test plan: scope, browsers, and exit criteria.
2. **Run the checklists.** Enter Pass, Fail, Blocked, or N/A for each item directly in the checklist.
3. **Add test cases and exploration** for anything the checklists don't cover. Record those runs in the execution log.
4. **Report bugs.** For each failure, copy `Bug-Report.md` into `bugs/` as `BUG-001.md`, `BUG-002.md`, and so on. Save screenshots in `evidence/`.
5. **Retest.** After a fix, run the check again and add a new row to the execution log.
6. **Summarize.** Total the results in the summary report and give a recommendation.

For a small change, steps 1 to 3 can be as short as "run the smoke checklist."

## Conventions

| Item | Format | Example |
|---|---|---|
| Smoke checklist items | `SMK-##` | SMK-04 |
| Regression checklist items | `REG-##` | REG-21 |
| Test cases | `TC-###` | TC-003 |
| Exploratory sessions | `EXP-###` | EXP-001 |
| Bugs | `BUG-###` | BUG-001 |
| Dates and cycle folders | `YYYY-MM-DD` / `YYYY-MM-short-name` | 2026-01-15 / 2026-01-homepage-redesign |
| Evidence files | `<ID>-<short-description>.png` | BUG-001-mobile-menu.png |

## Rules for Safe Records

- Never write real passwords, personal data, or customer information in any file.
- Crop or blur screenshots that show private details before you publish them.
- Mark a check as **Pass** only after you have run it.

## AI Transparency

This is an **AI-led** project. I set the goal, scope, and structure, and I review the changes. AI drafted the templates, checklists, and reference notes and helped revise them. Review each file and adapt it to your project before you rely on it.

## Contributing

Suggestions are welcome. Open an issue describing the change and why it would help.

## License

[MIT](LICENSE). You can use, copy, and change these files for any purpose, including commercial work.
