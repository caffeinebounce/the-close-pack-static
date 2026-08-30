# Skill: continuous close

Goal: post bank activity as it lands so month-end is a review.

## Cadence

- **Daily (or next banking day):** import new posted transactions.
- **Weekly:** clear uncategorized lines, match receipts, flag anything that needs a bill or invoice.
- **Month-end:** run the checklist and render the three-page package.

## Rules

1. Import **posted** activity only. Ignore pending cards.
2. One bank line becomes one ledger line (or a clear split you can explain).
3. Categories come from Mercury (or the CSV `category` column) first. Override only with a written reason in the note.
4. Owner draws, transfers, and loan activity are balance-sheet, not “miscellaneous expense.”
5. If you cannot classify a line in five minutes, put it on the exception list. Do not guess.

## Working file

Keep a single period sheet:

| date | bank_reference | amount | proposed_account | status | note |

Statuses: `imported`, `posted`, `exception`.

## Done when

Every posted bank line for the week is `posted` or `exception`, and cash in the ledger can be tied to the bank by reference.
