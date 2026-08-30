# Mercury token scopes

Use the smallest token that can read activity. This pack never initiates a payment.

## Allow

Create a Mercury custom token (or equivalent bank API credential) with **read** access to:

- **Categories** — so imported lines keep the category you already assigned in Mercury
- **Receipts** — so source images or attachments can be referenced in the ledger
- **Notes** — so memo text survives the import

That is enough to post a bank line and keep an audit trail.

## Deny

Do not enable:

- `SendMoney`
- ACH / wire / check initiation
- Recipient or payee writes
- Any scope that can create, approve, or release a payment

If the bank’s UI will not issue a token without a payment scope, stop and use a CSV export instead.

## CSV fallback

Export posted transactions for the period:

| date | amount | description | bank_reference | category | note |

Positive amounts are inflows. Negative amounts are outflows. Do not include pending authorizations.

## Rotation

Treat the token like a password. Store it in your own secret manager. Rotate it if a laptop is lost. Mosaiko LLC does not receive or store this token.
