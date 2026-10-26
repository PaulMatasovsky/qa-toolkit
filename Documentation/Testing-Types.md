# Testing Types and Techniques

*AI-generated reference notes; not a record of executed tests.*

## Common Testing Types

| Type | Purpose |
|---|---|
| Smoke | Quick check of critical functions after a change or deployment |
| Regression | Check previously working behavior after changes |
| Functional | Compare a feature's behavior with its requirements |
| Exploratory | Learn about the product while designing and executing tests |
| Integration | Check interactions between components or services |
| Acceptance / UAT | Determine whether business needs are satisfied |
| Accessibility | Evaluate whether people with disabilities can use the product |
| Performance | Examine responsiveness and behavior under load |
| Security | Assess potential risks to data, access, and system behavior |

## Example Test Design Techniques

**Equivalence partitioning:** Choose representative inputs from meaningful groups. For an age field accepting 1–120, example groups could be values below 1, from 1 to 120, and above 120.

**Boundary value analysis:** Test values at and around a limit. For a minimum password length of 8 characters, try lengths 7, 8, and 9.

**Exploratory testing:** Work from a focused test mission, record actions and observations, and adapt the next checks based on what is learned.

Use these notes to plan suitable tests; the presence of a testing type here does not mean it has been performed.
