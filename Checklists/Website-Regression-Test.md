# Website Regression Test

> A broader check that things which worked before still work after a change. Run it after a redesign, theme or plugin update, or a large content change.
> Select only the sections that apply to your site. Record each result in the [execution log](../Templates/Test-Execution-Log.md).
> Delete these instruction lines when you use the checklist.

- **Website / release:**
- **Change being tested:**
- **Date / tester:**
- **Browsers / devices:**
- **Environment:**

## Navigation and Content

- [ ] Main menu, footer menu, and breadcrumbs on every page.
- [ ] All internal links (no 404 pages) and external links.
- [ ] Search, if the site has one.
- [ ] Page titles and headings match the page content.
- [ ] Images, downloads, and embedded media.
- [ ] The 404 page appears for a made-up URL.

## Forms

- [ ] Required fields show a clear error when left empty.
- [ ] Invalid input (such as a bad email address) is rejected with a clear message.
- [ ] A valid submission shows a confirmation and reaches its destination (such as an inbox).
- [ ] Spam protection, if used, does not block real submissions.

## Accounts and Access (if the site has sign-in)

- [ ] Sign in, sign out, and password reset.
- [ ] Protected pages require sign-in.
- [ ] Each user role sees only what it should.

## Layout and Compatibility

- [ ] Layout, fonts, colors, buttons, and icons match the design.
- [ ] Pages work at phone, tablet, and desktop widths.
- [ ] Touch controls and mobile forms work.
- [ ] Each supported browser shows the same behavior.

## Accessibility

- [ ] All controls can be reached and used with the keyboard alone.
- [ ] A visible focus outline is shown on links, buttons, and form fields.
- [ ] Text meets color contrast requirements (WCAG AA: 4.5:1 for normal text, 3:1 for large text).
- [ ] Images that carry meaning have alt text. Decorative images have empty alt text.
- [ ] Each page has one main heading, and heading levels do not skip (H1, then H2, then H3).
- [ ] Form fields have visible labels.
- [ ] Content still works when the browser is zoomed to 200%.

## Performance and Technical

- [ ] Main pages load in a reasonable time on a mobile connection.
- [ ] The browser console shows no new errors, and no requests fail.
- [ ] HTTPS works on every page, with no mixed-content warnings.

## Result

- **Overall status:** Not run / Pass / Pass with issues / Fail
- **Skipped sections and why:**
- **Bug IDs:**
- **Retest needed:**
- **Notes:**
