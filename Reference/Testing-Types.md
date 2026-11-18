# Testing Types and Techniques

Use this page to choose which kinds of testing belong in your [test plan](../Templates/Test-Plan.md).

## Testing Types

| Type | Purpose |
|---|---|
| Smoke | Quick check of critical functions after a change or deployment |
| Regression | Check that previously working behavior still works after a change |
| Functional | Compare a feature's behavior with its requirements |
| Exploratory | Learn about the product while designing and running tests |
| Integration | Check how components or services work together |
| Acceptance (UAT) | Confirm that the product meets the business or user need |
| Accessibility | Check that people with disabilities can use the product |
| Performance | Check speed and behavior under load |
| Security | Check for risks to data, access, and system behavior |
| Data validation and reconciliation | Prove that every source record was loaded, rejected, or removed for a stated reason, and that loaded data matches the source |

## Test Design Techniques

**Equivalence partitioning:** Group inputs that should behave the same way, then test one value from each group. For an age field that accepts 1 to 120, the groups are below 1, 1 to 120, and above 120.

**Boundary value analysis:** Test values at and next to each limit. For a password with a minimum of 8 characters, test 7, 8, and 9 characters.

**Reconciliation:** Count records at each stage and confirm the numbers add up (rows in = rows loaded + rejected + removed). Then compare a few records field by field. Counts catch missing rows; spot checks catch wrong values.

**Seeded defects:** Plant known problems in test data, then measure how many your checks catch. It tells you how much to trust the checks, not just whether they ran.

**Exploratory testing:** Set a short goal (for example, "try to break the contact form"), record what you do and see, and let each result decide the next check.
