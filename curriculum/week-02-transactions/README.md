# Week 2 — Instructions, transactions and confirmation

**Time:** 90–120 minutes  
**Outcome:** a devnet transfer with readable simulation and confirmation UX.

## Resources

- [Solana transactions](https://solana.com/docs/core/transactions) — learn how instructions, signatures, and a recent blockhash fit together.
- [Solana Kit client guide](https://solana.com/docs/frontend/client) — see the current TypeScript client pattern for submitting transactions.

## Core task

Build a devnet-only transfer flow between two disposable learning addresses. Before signing, display the cluster, sender, recipient, amount, fee payer, simulation result, and estimated/known fee information. After sending, wait for confirmation and display a devnet explorer link.

## Acceptance criteria

- The amount is positive, bounded, and parsed safely.
- Mainnet is rejected.
- Simulation succeeds before signing.
- Confirmation uses a current blockhash strategy rather than a blind delay.
- Errors explain the likely next action.

## Stretch

Create one transaction containing two no-value instructions and explain atomicity by predicting what happens if one instruction fails.

## Project move

Write the project's primary transaction as instructions, required accounts, signers, and expected state changes.
