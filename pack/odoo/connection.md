# Odoo connection

This pack assumes **Odoo Accounting** for one company. Community or Enterprise is fine as long as you have journals, a chart of accounts, and bank reconciliation.

## Create the company

1. One company record. Do not reuse a database that already holds another entity’s books.
2. Fiscal year and tax settings that match your formation documents.
3. A chart of accounts you are willing to keep. Import a standard US chart if you are starting clean.

## Bank journal

1. Create a bank journal for the operating account.
2. Currency matches the Mercury (or bank) account.
3. Opening balance equals the bank statement on the day you start this pack.

## Import path

**Option A — CSV:** use the bank journal’s import / statement import with the columns in `skills/bank-csv-import.md`. Map `bank_reference` to the statement line’s unique id so reruns do not duplicate.

**Option B — Mercury token:** a small sync job (yours, not hosted by Mosaiko LLC) reads categories, receipts, and notes and writes statement lines onto that journal. No SendMoney scope.

## After connect

Post a single known transaction by hand. Confirm it lands on the right accounts. Then turn on the continuous-close skill.

## Out of scope

Multi-company databases, consolidation, and anyone else’s Odoo instance.
