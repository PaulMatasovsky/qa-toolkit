# Free Tools

These free tools help with the checklist items. Each one finds some problems automatically, but none replaces checking the site yourself.

| Tool | Use it for | Checklist items |
|---|---|---|
| Browser developer tools (F12) | Console errors, failed requests, mobile screen sizes | SMK-10, SMK-16, REG-16, REG-27 |
| [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview) (built into Chrome dev tools) | Performance, accessibility, and SEO scores | REG-26, REG-32 |
| [WAVE](https://wave.webaim.org/) | Accessibility errors shown on the page itself | REG-21 to REG-24 |
| [axe DevTools](https://www.deque.com/axe/devtools/) (browser extension) | Detailed accessibility issues with fix guidance | REG-21 to REG-24 |
| [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) | Checking one text and background color pair | SMK-13, REG-21 |
| [W3C Link Checker](https://validator.w3.org/checklink) | Broken links across a page | SMK-04, REG-02, REG-03 |

## Data Migration Tools

| Tool | Use it for | Checklist items |
|---|---|---|
| Google Sheets or Excel (COUNTIF, COUNTIFS, MATCH) | Counting rows, finding duplicates and orphans, reconciling totals | DMS-05, DMS-07, MIG-14 to MIG-17, MIG-23 |
| [Supabase](https://supabase.com/) free tier (PostgreSQL) | A real target database with a SQL editor and CSV import | DMS-09 to DMS-11, MIG-25, MIG-26 |
| [DB Browser for SQLite](https://sqlitebrowser.org/) | A local database for practice loads, with no account needed | DMS-09 to DMS-11, MIG-28, MIG-29 |

## Tips

- Test in a private or incognito window to see the site as a new visitor would, without your cache or sign-in.
- Take screenshots with the browser address bar visible, so the evidence shows which page you were on.
- Use synthetic or approved data with online tools. Never upload real personal or health information to a tool that isn't approved for it.
- Automated accessibility checkers catch only some issues. Keyboard and zoom checks (REG-19, REG-25) still need a person.
