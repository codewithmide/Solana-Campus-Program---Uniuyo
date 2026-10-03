# Week 4 — Rust for web developers

**Time:** 2 hours  
**Outcome:** a tested Rust model ready to become program logic.

## Resources

- [The Rust Book: ownership](https://doc.rust-lang.org/book/ch04-01-what-is-ownership.html) — the biggest new concept for most JavaScript developers.
- [The Rust Book: writing tests](https://doc.rust-lang.org/book/ch11-01-writing-tests.html) — use this while writing your success and error cases.

## Core task

Model a `Kudos` record with author, recipient, message, and timestamp-like input. Implement constructor validation, a message length limit, a rule preventing self-kudos, descriptive custom errors, and unit tests.

Focus on ownership/borrowing, structs/enums, `Result`, pattern matching, modules, and tests.

## Acceptance criteria

- `cargo fmt --check`, `cargo clippy`, and tests pass.
- Error variants are asserted in tests.
- No `unwrap()` is used on user-controlled input.
- Domain rules are separate from printing/CLI code.

## Stretch

Estimate serialized size and explain why bounded strings matter for account allocation.

## Project move

Implement and test the project's smallest domain rule in ordinary Rust before adding Anchor macros.
