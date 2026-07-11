Good Bug Report Example

Title

Login button becomes unresponsive after three failed login attempts

Severity: High

Priority: P1

⸻

Summary

After three consecutive failed login attempts, the Login button no longer responds to user input until the page is refreshed.

⸻

Environment

* Version: 1.2.0
* Browser: Chrome 138
* Windows 11

⸻

Preconditions

* User is on the login page.

⸻

Steps to Reproduce

1. Open the login page.
2. Enter an incorrect password.
3. Repeat three times.
4. Enter valid credentials.
5. Click Login.

⸻

Expected Result

The user should be able to log in successfully.

⸻

Actual Result

The Login button no longer responds.

⸻

Frequency

Always

⸻

Attachments

* Screenshot
* Browser console log

⸻

Notes

Refreshing the page restores normal behavior.