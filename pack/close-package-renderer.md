# Monthly three-page close package

Render one PDF (or print three pages) after the month-end checklist is done. Keep the package with the period’s trial balance.

## Page 1 — Profit and loss

- Revenue, cost of goods (if any), operating expenses, other income/expense, net income
- This month vs prior month
- One paragraph: what moved, in plain language
- Do not dump every account. Group to the P&L lines a CPA would expect

## Page 2 — Cash

- Opening cash, inflows, outflows, ending cash
- Bank balance vs ledger cash (the difference must be explained or zero)
- Large unusual outflows (transfers, owner draws, one-off vendors)
- If you use Mercury, note whether the token was categories/receipts/notes only

## Page 3 — Exceptions

A short table, not a novel:

| item | amount | why it is still open | owner | due |
| --- | --- | --- | --- | --- |
| Uncategorized bank lines |  |  |  |  |
| Unreconciled payments |  |  |  |  |
| Missing bills / receipts |  |  |  |  |
| Balance-sheet accounts that did not roll |  |  |  |  |

If the table is empty, write “No open exceptions” and stop. Do not invent commentary.

## Renderer notes

If you generate the pages from a script or a bot:

1. Pull posted P&L and cash for the closed period only.
2. Pull the exception list from the close working file, not from live bank pending.
3. Stamp the cover with entity name, period, and “draft” or “final.”
4. Archive the PDF next to the trial balance export.

The pack does not ship a hosted renderer. Keep the output on your machine.
