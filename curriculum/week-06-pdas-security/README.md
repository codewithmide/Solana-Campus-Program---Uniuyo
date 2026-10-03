# Week 6 — PDAs, constraints and defensive programs

**Time:** 2–3 hours  
**Outcome:** deterministic per-user state protected by explicit constraints.

## Resources

- [Anchor guide to PDAs](https://www.anchor-lang.com/docs/basics/pda) — derive addresses from seeds and validate them in your program.
- [Anchor account constraints reference](https://www.anchor-lang.com/docs/references/account-constraints) — look up signer, seeds, owner, and close rules.

## Core task

Extend the program so each user has deterministic state derived from documented seeds. Add update and close behavior with PDA derivation/bump handling, signer/owner/seed/relationship constraints, validation, custom errors, and hostile-account tests.

## Acceptance criteria

- Client and program derive the same address.
- Seeds include the intended namespace and identity.
- Unauthorized update/close fails.
- Wrong PDA, wrong owner, oversized data and duplicate initialization are tested.
- Close destination and reclaimed funds are intentional.

## Stretch

Add a safe CPI whose accounts and signer seeds are fully explained, then test the failure case.

## Project move

Threat-model assets/state at risk, trusted authorities, attacker-controlled inputs, and the three most important invariants.
