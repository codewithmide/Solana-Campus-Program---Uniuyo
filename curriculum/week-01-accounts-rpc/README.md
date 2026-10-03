# Week 1 — Accounts, programs and RPC

**Time:** 90–120 minutes  
**Outcome:** a TypeScript CLI that reads and explains onchain state.

The [first workshop account viewer and take-home challenge](../../workshops/01-first-steps/README.md) give you a working JavaScript starting point. Extend the watchlist here, or rebuild it in TypeScript.

## Resources

- [Solana core concepts](https://solana.com/docs/core) — start with Accounts and Programs to understand what your CLI will read.
- [Solana Kit client guide](https://solana.com/docs/frontend/client) — use this when you build the TypeScript RPC client.

## Mental model

A web2 server owns behavior and usually its database. On Solana, programs process instructions while accounts hold data. RPC lets a client read cluster state and submit transactions.

## Core task

Build a CLI that accepts at least two public addresses and prints a result for each:

- selected cluster and RPC endpoint name (never a secret URL);
- balance in lamports and SOL;
- whether account data exists;
- account owner when present;
- an explorer link for the selected cluster.

Handle an invalid address and RPC failure with useful messages while still showing the other results.

## Acceptance criteria

- Address input is validated before the request.
- Lamports-to-SOL conversion does not silently lose precision.
- Cluster is explicit and defaults to devnet.
- One command shows at least two address results.
- A bad address does not hide a valid address's result.
- The command and sample output are saved in your README.

## Stretch

Use `getMultipleAccounts` to fetch addresses in one RPC call, then compare executable program accounts with ordinary data accounts.

## Project move

Draw the project account model: what data exists, who owns each account, who may update it, and who must sign.
