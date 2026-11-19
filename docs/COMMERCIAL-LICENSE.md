# Nivora Production-Use License (draft for review by Zyvor AI Labs Private Limited and its counsel)

Nivora is source-available under the Zyvor Production License v1.0 (`LICENSE`). Non-production use is free. Under
section 4 of that licence, Production Use needs a separate written commercial license from Zyvor AI Labs Private
Limited. This page describes the one-time paid grant that is that commercial license for Nivora, covering
**production use, including business and commercial use**.

## Free use

Anyone may use Nivora for Non-Production Use (as defined in `LICENSE`) without paying: build it from source, use the
unsigned build from GitHub Releases, or run the collector. Use that supports live business operations, employees,
customers or revenue is Production Use and needs the paid grant.

## The paid grant

On receipt of payment for a Nivora build (₹999 including GST, about US$12, per build), Zyvor AI Labs Private Limited
("Licensor") grants the payer ("Licensee", an individual or a single legal entity) a perpetual, worldwide,
non-exclusive, non-transferable licence to:

1. use Nivora for Production Use, including business and commercial purposes, on machines the Licensee owns or operates;
2. do so for the version bought and every later version released by Licensor under the Zyvor Production License v1.0 or a successor Zyvor licence;
3. modify the source for the Licensee's own use.

## What it does not cover

- Redistribution, sublicensing, reselling, or hosting Nivora as a product or service for third parties.
- Redistribution rights beyond section 8 of `LICENSE`, which requires prior written permission.
- Removing licence notices (`LICENSE`, SPDX headers).
- More than one legal entity: affiliates and customers need their own grant.
- A warranty that the **developer build's** content filter or capture helper can be activated: they need Apple
  entitlements and a provisioning profile that the Licensee must obtain, and they are compile-verified only.

## Proof and terms

- The invoice or payment receipt is the proof of a paid grant. Earlier paid grants are perpetual and need no key.
- From 0.5.4 the app can read an optional licence key (`ZYV1.…`, a signed 30-day trial key or a licence key issued by Zyvor) under **Nivora > Licence…**. The key is verified offline with a public key built into the app, stored in the macOS Keychain (with a user-only file fallback), and used only to show the licence status. Enforcement is soft: nothing is disabled without a key or after a key expires, there is no network check and no hardware binding. A free 30-day trial key is available from sales@zyvor.dev; licences are obtained at https://zyvor.dev/buy.
- Provided as is, no warranty, under the same disclaimers as the Zyvor Production License v1.0. Payments are non-refundable except as
  required by law.
- Prices on this page are drafts pending owner approval.
- Questions, receipts, new download links, and larger or multi-entity licences: sales@zyvor.dev.
- Governing law and venue: *[Licensor and counsel to fill in]*. Tax and GST treatment: *[Licensor and counsel to fill in]*.

## Open questions for counsel

- Whether ₹999 is intended to cover large organisations or should be capped by entity size.
- The exact line between Non-Production and Production Use for individuals running Nivora on their own Mac, and for freelancers and employees using it at work.
- Transferability on a company sale, and what happens to prior payers if terms change.
