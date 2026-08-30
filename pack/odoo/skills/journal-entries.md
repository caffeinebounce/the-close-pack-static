# Skill: Odoo journal entries

## Bank statement lines

Create statement lines on the operating bank journal. Do not book random miscellaneous journal entries for ordinary bank activity.

Each line needs:

- Date (posted date)
- Amount
- Partner if you have one (vendor or customer)
- Counterpart account from your category map
- The Mercury / CSV `bank_reference` in the label or narration

## Non-bank entries

Use a miscellaneous journal only for:

- Opening balances
- Depreciation or prepaid amortization
- Corrections you can explain in the narration

Every miscellaneous entry gets a narration that a stranger could audit.

## Owner activity

Draws and contributions go to equity accounts. Do not expense personal charges and “fix it later.”

## Idempotency

Before posting, search the journal for the `bank_reference`. If it exists, skip. Duplicate posts are the usual way a close goes sideways.
