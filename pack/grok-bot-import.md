# Optional Grok Bot import

The Close Pack works as markdown you read and follow. You do not need a bot.

If you want a Grok Bot to apply the skills, import them as **instructions and knowledge**, not as credentials.

## What to import

Upload these files as knowledge (or paste them into custom instructions):

- `skills/continuous-close.md`
- `skills/bank-csv-import.md`
- `skills/month-end-checklist.md`
- `close-package-renderer.md`
- The ledger skill folder you bought (`odoo/skills/` or `quickbooks/skills/`)

Keep `mercury-scopes.md` in the instructions so the bot refuses payment scopes.

## System note to paste

Use this as a standing instruction:

> You help one company close its own books. You do not ask for SendMoney or any payment-initiation token. You do not ask for anyone else’s books. You do not invent balances. If a figure is missing, say so and add it to the exception list.

## What not to paste

- API tokens
- Bank login passwords
- Live vendor lists or payroll files from another entity
- Private close notes that are not yours

## After import

Run one dry month: ask the bot to produce the three-page package from a CSV you already reviewed. Compare it to your ledger. If the bot wants a broader Mercury scope, the import is wrong — fix the instructions, not the token.
