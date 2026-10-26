# Sample Login Test Scenarios

**AI-generated, unexecuted examples.** These assume an application with a login page. They are not findings from the portfolio website.

| ID | Scenario | Expected behavior |
|---|---|---|
| TC-001 | Enter valid credentials | User signs in and reaches an authorized page |
| TC-002 | Enter an invalid password | Access is rejected with an appropriate message |
| TC-003 | Leave username blank | Input is rejected or appropriate validation appears |
| TC-004 | Leave password blank | Input is rejected or appropriate validation appears |
| TC-005 | Use Remember Me, if supported | Session behavior matches requirements |
| TC-006 | Log out | Session ends and protected pages require reauthentication |

Before execution, add environment, preconditions, steps, test accounts, and evidence using the [test case template](Test-Case-Template.md). Never publish real passwords or sensitive account data.
