# Data Migration Smoke Test

> A quick check that a data load worked before anyone relies on it. Run it after every load or reload, including practice runs. It usually takes 10 to 15 minutes.
> If any check fails, stop and fix the pipeline before running the full [Data Migration Validation](Data-Migration-Validation.md) checklist.
> Mark each item **N/A** if it does not apply, and add rows for anything specific to your data. Enter a **Bug ID** for every **Fail**.
> Delete these instruction lines when you use the checklist.

- **Migration / load run:**
- **Source file(s) and export date:**
- **Target system:**
- **Date / tester:**

**Result values:** Pass · Fail · Blocked · N/A

## Source

| ID | Check | Result | Bug ID |
|---|---|---|---|
| DMS-01 | The source file is the expected export (right name, date, and system) and opens without errors. | | |
| DMS-02 | The source row count matches what the source system or client says it exported. | | |
| DMS-03 | Every required source column is found and mapped. Nothing shows as missing or #N/A in the header mapping. | | |

## Transformation

| ID | Check | Result | Bug ID |
|---|---|---|---|
| DMS-04 | The output contains no error values (#N/A, #VALUE!, #REF!, NULL where a value is required). | | |
| DMS-05 | Rows in = rows out + rows rejected + rows removed. Every row is accounted for. | | |
| DMS-06 | Every rejected or removed row has a reason recorded. | | |
| DMS-07 | Record IDs in the output are unique. | | |
| DMS-08 | No test, sample, or placeholder records are in the output. | | |

## Load

| ID | Check | Result | Bug ID |
|---|---|---|---|
| DMS-09 | The import into the target finishes without errors or skipped rows. | | |
| DMS-10 | Row counts in the target match the output file, table by table. | | |
| DMS-11 | Every child record (such as an appointment) points to a parent record (such as a client) that exists. | | |
| DMS-12 | Three records picked at random look the same in the source, the output, and the target. | | |

## Result

- **Overall status:** Not run · Pass · Fail · Blocked
- **Counts:** In ___ · Loaded ___ · Rejected ___ · Removed ___ · Flagged ___
- **Items marked N/A or Blocked, and why:**
- **Notes:**
