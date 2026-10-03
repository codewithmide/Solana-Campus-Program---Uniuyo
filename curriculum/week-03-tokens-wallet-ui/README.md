# Week 3 — Tokens and wallet-connected UI

**Time:** 2 hours  
**Outcome:** a small web app that connects a wallet and displays devnet assets.

## Resources

- [Solana React guide](https://solana.com/docs/frontend/react-hooks) — wallet connection and chain data in React.
- [Solana token basics](https://solana.com/docs/tokens/basics) — understand token mints and token accounts before displaying balances.

## Core task

Create a page that discovers supported wallets using the current cohort starter, connects/disconnects explicitly, shows the public address and cluster, reads SOL/token balances, handles loading/empty/error/success states, and links to the devnet explorer.

No seed phrase or private key should ever enter the app.

## Acceptance criteria

- Wallet state survives normal component rerenders.
- Buttons cannot submit twice while pending.
- Addresses are shortened visually but available in full.
- Cluster is visible near every signing action.
- Empty and error states are usable, not blank screens.

## Stretch

Add a devnet token transfer behind a transaction review panel and identify which token program owns the mint/account.

## Project move

Produce a clickable happy path, even if its program call is still mocked.
