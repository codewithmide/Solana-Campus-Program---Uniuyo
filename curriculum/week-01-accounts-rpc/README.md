# Week 1 — Accounts, programs and RPC

**Time:** 90–120 minutes  
**Outcome:** a TypeScript CLI that reads and explains onchain state.

## Resources

- [Solana core concepts](https://solana.com/docs/core) — start with Accounts and Programs to understand what your CLI will read.
- [Solana Kit client guide](https://solana.com/docs/frontend/client) — use this when you build the TypeScript RPC client.

## Mental model

A web2 server owns behavior and usually its database. On Solana, programs process instructions while accounts hold data. RPC lets a client read cluster state and submit transactions.

## Core task

Build a CLI that accepts a public address and prints:

- selected cluster and RPC endpoint name (never a secret URL);
- balance in lamports and SOL;
- whether account data exists;
- account owner when present;
- an explorer link for the selected cluster.

Handle an invalid address and RPC failure with useful messages.

## Acceptance criteria

- Address input is validated before the request.
- Lamports-to-SOL conversion does not silently lose precision.
- Cluster is explicit and defaults to devnet.
- Output for at least two addresses is saved in the README.

## Stretch

Fetch multiple accounts efficiently and compare executable program accounts with ordinary data accounts.

## Project move

Draw the project account model: what data exists, who owns each account, who may update it, and who must sign.
