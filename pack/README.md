# Close Pack

Sold by Mosaiko LLC. This folder is a generic close playbook for **one company that you own**. It is not a bookkeeping service and it does not include anyone else’s books.

## What you just bought

- Markdown skills for a continuous close
- A monthly three-page close-package renderer
- Mercury (or bank CSV) import notes
- Ledger connection notes for the SKU you paid for (Odoo, QuickBooks Online, or both)
- Optional Grok Bot import notes

## Layout

```
pack/
  README.md
  mercury-scopes.md
  close-package-renderer.md
  grok-bot-import.md
  skills/
    continuous-close.md
    month-end-checklist.md
    bank-csv-import.md
  odoo/
    connection.md
    skills/
      journal-entries.md
      reconciliation.md
  quickbooks/
    connection.md
    skills/
      journal-entries.md
      reconciliation.md
```

Odoo SKU: shared files plus `odoo/`. QuickBooks SKU: shared files plus `quickbooks/`. Bundle: this whole folder.

## What you need before the start

1. One legal entity and one operating bank account.
2. A ledger you already use: Odoo Accounting **or** QuickBooks Online.
3. Either a Mercury developer token limited to the scopes in `mercury-scopes.md`, **or** a monthly bank CSV export.
4. An opening trial balance you trust. Do not start mid-mess and hope the pack reconstructs history.

## Safe bank access

If you connect Mercury, create a token that can read **categories, receipts, and notes only**. Never grant `SendMoney` or any payment-initiation permission. The pack has no reason to move cash.

CSV fallback: export posted transactions (date, amount, description, bank reference) and follow `skills/bank-csv-import.md`.

## Suggested order

1. Read `mercury-scopes.md`.
2. Connect the ledger (`odoo/connection.md` or `quickbooks/connection.md`).
3. Run `skills/continuous-close.md` for two weeks.
4. At month-end, use `skills/month-end-checklist.md` and `close-package-renderer.md`.
5. Optional: `grok-bot-import.md` if you want the skills loaded into a Grok Bot.

## License in one line

Use and adapt these files for one company. Do not resell the pack.
