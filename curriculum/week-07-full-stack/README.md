# Week 7 — Full-stack dApp and transaction UX

**Time:** 2–3 hours  
**Outcome:** an end-to-end devnet MVP another student can use.

## Resources

- [Solana React guide](https://solana.com/docs/frontend/react-hooks) — connect your interface to wallet and RPC state.
- [Anchor clients](https://www.anchor-lang.com/docs/clients) — call your program from a typed client.

## Core task

Connect the frontend to the program's typed client. Show wallet/cluster/action before signing, simulate when supported, distinguish rejection/simulation/submission/confirmation, refresh state, link Explorer, avoid double submission, and validate returned account ownership/shape.

## Acceptance criteria

- A new tester can complete the happy path from the README.
- One failed transaction is recoverable without reloading.
- Loading and confirmation states are accurate.
- Program ID and cluster configuration are explicit.
- Core UI logic has tests; program tests still pass.

## Stretch

Add structured client errors, signature capture, and a privacy-conscious way for testers to report failures.

## Project move

Reach feature freeze. Fix the happy path and two important failure paths; defer unrelated features.
