# ProofCart AI

Sponsored by **CREIGNIFICENT LLC**.

Know what changed hands. Before the money does.

Create a timestamped evidence record for person-to-person purchases using photos, seller disclosures, and AI-assisted organization.

**AI organizes evidence. People approve facts. ProofCart does not guarantee authenticity or condition.**

## Open the V1 demo

Open [`index.html`](./index.html) in a browser. No build step.

This is a local walkthrough: used electronics only. No accounts, no uploads, no Stripe, no model calls.

## What this is

Buyer and seller create a verifiable **condition evidence package** immediately before money changes hands (Marketplace, OfferUp, Craigslist, used electronics).

AI may say: “A scratch appears visible on the lower-right corner in image 4.”

AI may not say: “This laptop is in excellent condition.”

## Agent loop

Capture → Extract → Compare → Flag uncertainty → Seller confirms → Buyer reviews → Human approval → Payment → Immutable snapshot → Audit

AI cannot change price, accept evidence for the seller, acknowledge for the buyer, issue refunds, or mark payment successful.

## V1 scope

In: used electronics, evidence checklist, AI organization with provenance, seller correction, locked proof record, buyer acknowledgment, Stripe Checkout + signed webhook (production), receipt, append-only audit.

Out: marketplace scraping, valuation, escrow, shipping, fraud insurance, authenticity certificates, dispute adjudication, reputation scores, automated refunds.

## Monetization hypothesis

Free drafts. **$4.99** per completed evidence package. First test: 20 local electronics sales. If nobody pays, do not build marketplace integrations.

## Production stack (not this commit)

Next.js + TypeScript + Tailwind · Vercel · Firebase Auth / Firestore / Storage · Gemini multimodal · Stripe Checkout + webhooks · Resend · Zod · Vitest + Playwright

## Security posture

Zero Trust: authenticated identity, transaction-scoped authorization, private storage, least privilege, schema validation, upload quarantine, prompt injection treated as untrusted content, signed webhooks, idempotent event IDs, serial numbers not public, no model training on customer evidence without consent.

## Definition of done

Two unrelated users can create accounts, capture electronics evidence, correct AI output, lock the record, keep strangers out, record buyer acknowledgment, complete a Stripe **test** purchase, verify the webhook once, and keep the receipt after refresh.

No fake payments. No fake AI analysis. No fake verification badges.
