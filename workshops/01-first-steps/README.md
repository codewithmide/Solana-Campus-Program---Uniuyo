# First workshop: your first Solana read

This workshop is for individual builders. You will create a practice wallet, inspect an account on devnet, and run a small JavaScript program that reads live account data.

**You need:** a laptop, Node.js 20 or newer, and internet access. No paid RPC account is required. If you already have a devnet wallet, you can use its public address.

## Exercise 1 — Make a practice wallet

1. Follow the [Solana Quick Start](https://solana.com/docs/intro/quick-start) to create a Solana Playground wallet and connect to **devnet**.
2. Copy your **public address**. Do not copy or share your recovery phrase or private key.
3. Open `https://explorer.solana.com/address/YOUR_ADDRESS?cluster=devnet`, replacing `YOUR_ADDRESS` with your public address.
4. Get devnet test SOL through the Quick Start's faucet instructions. If the faucet is slow or rate limited, continue with Exercise 2 using the example address below.

**Show your result:** your address page on Solana Explorer with devnet selected.

## Exercise 2 — Read an account with JavaScript

From this directory, run:

```bash
node account-viewer.mjs 11111111111111111111111111111111
```

The example address is the System Program. Then run the script with your own **public** address:

```bash
node account-viewer.mjs YOUR_ADDRESS
```

Compare the script output with Solana Explorer. Find the balance in lamports and SOL, the account owner, and whether the account is executable. If your wallet has no activity yet, note how the script describes an account that does not exist onchain.

**Show your result:** your terminal output and the matching devnet explorer page.

## During the workshop: make it yours

Change one part of the output so a new student can understand it more easily. Ideas: explain what a lamport is, label executable accounts as programs, or add a short message when an address has no onchain data yet. Run the script again and show your change.

## Before the next build night: your own challenge

Turn the single-address viewer into a **devnet account watchlist**. This is your individual task after the workshop:

1. Let the command accept **two or more public addresses**.
2. Fetch each account and print a compact summary for each: address, SOL balance (or “not found”), owner, and whether it is executable.
3. Keep a bad address or failed RPC request from hiding the results for the other addresses.
4. Add a short `README.md` to your own repository with the command to run your watchlist and one thing you learned about the accounts you inspected.

Try your own devnet address and the System Program address. Check both in Explorer. At the October 22 build night, bring your repository and show the command running, even if one part is still unfinished.

**Done when:** one command displays results for at least two addresses, and a bad address produces a useful message without stopping the other result.

**Hint:** `process.argv.slice(2)` gives you all command-line arguments. You can reuse `getAccountInfo`, `describeAccount`, and `Promise.allSettled` from JavaScript. The [Week 1 challenge](../../curriculum/week-01-accounts-rpc/README.md) takes this further.

## If something goes wrong

- `node: command not found`: install Node.js 20+ or use a machine with Node installed.
- `Invalid address`: copy the full public address without spaces or punctuation.
- `HTTP 429` or a temporary RPC error: wait briefly and retry. The public devnet RPC is rate limited. A free-tier devnet RPC can be used by setting `SOLANA_DEVNET_RPC_URL`, but make sure it actually points to devnet.
- Faucet unavailable: use the System Program address above for Exercise 2 and retry the faucet later.

## Read more

- [Solana accounts](https://solana.com/docs/core/accounts)
- [Solana JSON-RPC overview](https://solana.com/docs/rpc/http)
- [Solana clusters and public RPC endpoints](https://solana.com/docs/references/clusters)
