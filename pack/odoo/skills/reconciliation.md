# Skill: Odoo reconciliation

## Bank

1. Open the bank journal reconciliation.
2. Match statement lines to counterpart entries (vendor bills, customer invoices, or the counterpart you posted on import).
3. Leftover lines become exceptions, not forced matches.

## Bills and invoices

- A vendor bill should exist before you match a payment, unless the charge is a simple expense with a receipt.
- Customer receipts match open invoices by amount and partner. Partial payments stay open.

## Period lock

When the three-page package is `final`, lock the period (or at least the bank journal) so next month cannot rewrite this one.

## Common breaks

- Pending card settled in the next period — belongs next period
- Mercury category says “Software,” ledger says “Contractor” — pick one and document the override
- Transfer to a savings account booked as expense — move it to an asset
