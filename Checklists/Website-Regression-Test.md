# Website Regression Test

> A broader check that things which worked before still work after a change. Run it after a redesign, a theme or plugin update, or a large content change.
> Delete sections that do not apply, and mark single items **N/A**. Enter a **Bug ID** for every **Fail**.
> Delete these instruction lines when you use the checklist.

- **Website / release:**
- **Change being tested:**
- **Date / tester:**
- **Browsers / devices:**
- **Environment:**

**Result values:** Pass · Fail · Blocked · N/A

## Navigation and Content

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-01 | Main menu, footer menu, and breadcrumbs work on every page. | | |
| REG-02 | Internal links do not lead to 404 pages. | | |
| REG-03 | External links open the right destination. | | |
| REG-04 | Site search returns relevant results, if the site has search. | | |
| REG-05 | Page titles and headings match the page content. | | |
| REG-06 | Images, downloads, and embedded media load. | | |
| REG-07 | A made-up URL shows the site's 404 page. | | |

## Forms

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-08 | Required fields show a clear error when left empty. | | |
| REG-09 | Invalid input (such as a bad email address) is rejected with a clear message. | | |
| REG-10 | A valid submission shows a confirmation. | | |
| REG-11 | The submission arrives at its destination (such as an inbox), not in spam. | | |

## Accounts and Access (sites with sign-in)

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-12 | Sign in, sign out, and password reset work. | | |
| REG-13 | Protected pages require sign-in. | | |
| REG-14 | Each user role sees only what it should. | | |

## Layout and Compatibility

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-15 | Layout, fonts, colors, buttons, and icons match the design. | | |
| REG-16 | Pages work at phone, tablet, and desktop widths. | | |
| REG-17 | Touch controls and mobile forms work. | | |
| REG-18 | Each supported browser shows the same behavior. | | |

## Accessibility

See [Free Tools](../Reference/Free-Tools.md) for checkers that help with these items.

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-19 | All controls can be reached and used with the keyboard alone. | | |
| REG-20 | A visible focus outline shows on links, buttons, and form fields. | | |
| REG-21 | Text meets WCAG AA contrast: 4.5:1 for normal text, 3:1 for large text. | | |
| REG-22 | Meaningful images have alt text. Decorative images have empty alt text. | | |
| REG-23 | Each page has one main heading, and heading levels do not skip. | | |
| REG-24 | Form fields have visible labels. | | |
| REG-25 | Content still works with the browser zoomed to 200%. | | |

## Performance and Technical

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-26 | Main pages load in a reasonable time on a mobile connection. | | |
| REG-27 | The browser console shows no new errors, and no requests fail. | | |
| REG-28 | Every page uses HTTPS with no mixed-content warnings. | | |

## Content Management Systems (WordPress and similar)

| ID | Check | Result | Bug ID |
|---|---|---|---|
| REG-29 | Changes appear for signed-out visitors after the site and browser caches are cleared. | | |
| REG-30 | Theme templates (header, footer, blog posts, 404 page) display correctly. | | |
| REG-31 | Plugins still work after theme or plugin updates. | | |
| REG-32 | Page titles and meta descriptions are set on main pages. | | |
| REG-33 | Unpublished drafts and test pages are not visible to the public. | | |

## Result

- **Overall status:** Not run · Pass · Pass with issues · Fail
- **Sections or items skipped, and why:**
- **Retest needed:**
- **Notes:**
