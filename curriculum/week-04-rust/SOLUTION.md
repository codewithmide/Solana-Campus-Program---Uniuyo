# Week 4 — Reference solution

Use a `Kudos` struct and `KudosError` enum. Make construction return `Result<Kudos, KudosError>`. Validate identity and length before creating the value.

Tests cover valid creation, self-kudos, empty text, boundary length, and one character over the boundary. Note that UTF-8 byte length and displayed character count are not always identical.

The goal is learning to make invalid states and failure behavior explicit before code reaches the chain.
