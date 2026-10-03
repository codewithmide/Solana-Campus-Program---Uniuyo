# Week 6 — Reference solution

Use a stable namespace plus the user's public key as seeds when the invariant is one record per user. Store or validate the bump consistently. Constraints express authority/account relationships at the boundary; handler logic enforces domain rules.

Negative tests should provide a valid account in the wrong role; malformed data alone is not a strong authorization test. Verify state and lamport changes after close.

A passing suite is evidence that tested behavior works, not a security audit. Document assumptions and untested invariants.
