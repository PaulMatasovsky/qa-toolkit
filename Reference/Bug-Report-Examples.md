# Bug Report Examples

These examples are fictional. They show the difference between a report someone can act on and one they cannot. Use the [bug report template](../Templates/Bug-Report.md) for real reports.

## Too Vague

> **Title:** Login broken
>
> **Description:** Login doesn't work.

The reader cannot tell where it happened, what steps caused it, or what was expected.

## Useful

**BUG-001: Login button stops responding after three failed attempts**

- **Environment:** Staging, Chrome 120 on Windows 11
- **Severity:** High
- **Priority:** P1
- **How often:** Always
- **Preconditions:** A test account exists.

**Steps to reproduce:**

1. Open the login page.
2. Submit an incorrect password three times.
3. Enter the correct test credentials.
4. Select **Login**.

**Expected result:** The user signs in, or a clear message explains why they cannot.

**Actual result:** The Login button does nothing until the page is refreshed. No error message appears.

**Evidence:** Screen recording and a screenshot of the browser console.

## What Makes It Useful

- The title says what fails and when.
- The steps can be repeated by someone else.
- Expected and actual results are stated separately.
- The environment and evidence let a developer start without asking questions.
