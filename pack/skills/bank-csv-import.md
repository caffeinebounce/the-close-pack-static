# Skill: bank CSV import

Use this when you do not have a Mercury token, or when you want a paper trail beside the API.

## File

One CSV per account per period. UTF-8. Header row required:

`date,amount,description,bank_reference,category,note`

- `date` — ISO `YYYY-MM-DD` in the bank’s posted date
- `amount` — signed; inflows positive
- `bank_reference` — the bank’s immutable id, not the memo
- `category` / `note` — optional; preserve if present

Reject the file if two rows share a `bank_reference`.

## Steps

1. Export from Mercury or the bank after the previous period is closed.
2. Drop pending and intra-day holds.
3. Map `category` to your chart of accounts. Unknown categories become exceptions, not “Ask My Accountant” forever.
4. Post in the ledger using the bank journal / bank feed for that account.
5. Store the CSV next to the close package. Do not overwrite last month’s file.

## Mercury users

If you also have a read-only token, treat CSV as the backup. The token still must stay limited to categories, receipts, and notes.
