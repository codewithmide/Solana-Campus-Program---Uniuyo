# Week 2 — Reference solution

Use a five-stage flow: validate → build → simulate → review/sign → confirm.

Do not mix UI formatting with transaction construction. Return a review object containing cluster, fee payer, signers, destination, amount, and instruction count. The UI renders this object before any wallet prompt.

Tests should prove that invalid amounts and mainnet are rejected, simulation failure prevents signing, and a failed/expired confirmation produces a recoverable error. “Signature returned” is not the same as “transaction confirmed.”
