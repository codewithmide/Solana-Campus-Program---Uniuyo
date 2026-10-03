# Week 1 — Reference solution

Structure the CLI as small functions: `parseAddress`, `fetchAccount`, `formatBalance`, and `explorerUrl`. Inject the RPC client so tests can use a fake response.

Key checks:

- Reject malformed input before calling RPC.
- Keep lamports as an integer/bigint representation for calculations and format SOL only for display.
- Treat a missing account as a valid result, not a crash.
- Never assume returned account data belongs to the expected program; compare the owner first.

Test the formatter, invalid input, missing account, and RPC error paths.
