# Week 3 — Reference solution

Separate wallet discovery/connection, chain reads, and presentation. Model request state explicitly (`idle`, `loading`, `success`, `empty`, `error`) and disable repeated actions while pending.

Never infer token type solely from UI metadata. Validate mint/token-account ownership and distinguish the original SPL Token program from Token-2022 when constructing instructions.

Test disconnected, connected-empty, populated, rejected-wallet, and RPC-error states with a fake client/provider.
