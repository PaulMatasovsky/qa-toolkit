# Data Migration Validation

> A full check that migrated data is complete, correct, and usable. Run it once the [Data Migration Smoke Test](Data-Migration-Smoke-Test.md) passes, before the data is signed off or the old system is switched off.
> Write down the business rules first (what gets fixed, flagged, rejected, or removed). Many checks below compare the data against those rules.
> Delete sections that do not apply, and mark single items **N/A**. Enter a **Bug ID** for every **Fail**.
> Delete these instruction lines when you use the checklist.

- **Migration / release:**
- **Source system and export date:**
- **Target system:**
- **Business rules:** (link)
- **Date / tester:**

**Result values:** Pass · Fail · Blocked · N/A

## Mapping

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-01 | Every target field has a documented source field, or a documented reason it's left blank. | | |
| MIG-02 | Source fields that are not migrated are listed on purpose, not dropped by accident. | | |
| MIG-03 | Renaming or reordering source columns does not change the output. | | |
| MIG-04 | Values that need translating (status codes, provider names, abbreviations) map to one approved value each. No unmapped values remain. | | |

## Formats

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-05 | Dates in every source format convert to the same correct date. Spot-check one of each format. | | |
| MIG-06 | Two-digit years land in the right century. | | |
| MIG-07 | Leading zeros survive in codes and ZIP codes. | | |
| MIG-08 | Phone numbers, emails, and times are in one standard format. | | |
| MIG-09 | Extra spaces, odd capitalization, and invisible characters are removed from names and IDs. | | |
| MIG-10 | Numbers stored as text (such as "$25.00" or "50 min") convert to numbers. | | |

## Required Fields and Limits

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-11 | Rows missing a required field are rejected with that reason. | | |
| MIG-12 | Values at each limit pass, and values just outside fail (for example, durations of 14, 15, 180, and 181 minutes). | | |
| MIG-13 | Impossible values are caught: dates that don't exist, birth dates in the future, negative amounts. | | |

## Duplicates and Identity

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-14 | Exact duplicate rows are removed and counted. | | |
| MIG-15 | Likely duplicates (same name and birth date, different ID) are flagged for a person to review, not merged automatically. | | |
| MIG-16 | One ID used for two different records is caught. | | |

## Relationships

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-17 | Child records whose parent doesn't exist (orphans) are rejected with that reason. | | |
| MIG-18 | Child records whose parent was rejected are handled by a stated rule. | | |
| MIG-19 | Records that contradict each other are flagged (for example, an appointment before the client's intake date, or a double-booked provider). | | |

## Business Rules

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-20 | Each fix, flag, reject, and remove rule produces the result the business rules describe. | | |
| MIG-21 | Statuses make sense for their dates (for example, no future appointment marked Completed). | | |
| MIG-22 | Flagged rows load and appear on a follow-up list with a reason. | | |

## Load and Reconciliation

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-23 | Row counts reconcile at every stage: source, cleaned, loaded, rejected, removed. | | |
| MIG-24 | Totals that should not change, such as total copays or completed appointments, match between source and target. | | |
| MIG-25 | Database checks (keys, required fields, allowed values) accept every loaded row. | | |
| MIG-26 | A deliberately bad row is refused by the target, which proves the database checks work. | | |
| MIG-27 | Ten records picked at random match field by field between source and target. | | |

## Rerun

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-28 | Running the same export again gives the same output. | | |
| MIG-29 | Reloading into the target does not create duplicate records. | | |

## Privacy and Access

| ID | Check | Result | Bug ID |
|---|---|---|---|
| MIG-30 | Only approved or synthetic data is used outside the production system. | | |
| MIG-31 | Working files, exports, and screenshots containing personal data are stored and shared only where approved. | | |
| MIG-32 | Access to the target data is limited to the people who need it. | | |

## Result

- **Overall status:** Not run · Pass · Pass with issues · Fail
- **Counts:** In ___ · Loaded ___ · Rejected ___ · Removed ___ · Flagged ___
- **Sections or items skipped, and why:**
- **Open flags handed to the business:**
- **Retest needed:**
- **Notes:**
