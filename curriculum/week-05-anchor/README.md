# Week 5 — Anchor programs and persistent state

**Time:** 2–3 hours  
**Outcome:** a locally tested and devnet-deployed minimal program.

## Resources

- [Anchor local development quick start](https://www.anchor-lang.com/docs/quickstart/local) — create, build, test, and deploy your first program.
- [Anchor program structure](https://www.anchor-lang.com/docs/basics/program-structure) — identify instructions, state, and account validation.

## Core task

Implement an Anchor counter or guestbook with initialize and update instructions. Define state and allocated size, payer/signer, system program interaction, authority rule, useful logs, and happy/negative tests.

## Acceptance criteria

- Build and local tests pass using the pinned Anchor version.
- Account space calculation is explained.
- At least two negative tests assert specific errors.
- Devnet program ID and one explorer transaction are documented.
- Upgrade authority and its implications are recorded.

## Stretch

Generate a typed client from the IDL rather than hand-writing account codecs.

## Project move

Create the program skeleton and implement one complete state transition with tests.
