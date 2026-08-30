# QuickBooks Online connection

This pack assumes **one QuickBooks Online company**. Plus or Advanced is enough. Do not point this playbook at a firm file that already holds other clients.

## Company setup

1. Legal name, EIN, and address match your formation documents.
2. First month of fiscal year is correct.
3. Chart of accounts is the one you will keep. Turn on account numbers if you want a stable map from Mercury categories.

## Bank

1. Add the operating bank account (Mercury or other).
2. Opening balance equals the bank on the start date.
3. If you use the QBO bank feed, review — do not auto-add — until the category map is trusted.

## Import path

**Option A — CSV:** Banking → Upload transactions. Use the columns in `skills/bank-csv-import.md`. Keep `bank_reference` in the memo or a custom field so reruns are visible.

**Option B — Mercury token:** a small sync you run yourself writes expenses/deposits using read-only categories, receipts, and notes. No SendMoney scope. Mosaiko LLC does not host this sync.

## Classes / locations

Optional. If you use classes, map them in the category table. Do not invent a class for every vendor.

## After connect

Manually add one known coffee or software charge. Confirm the register and the P&L. Then start the continuous-close skill.

## Out of scope

QuickBooks Desktop, accountant-firm client files, and payroll filings.
