# Week 5 — Reference solution

Separate instruction handlers, state, errors, and constants. Initialization pays for a correctly sized state account; update requires the stored authority to sign.

Tests must read state after each instruction rather than treating a returned signature as proof. Include initialization, successful update, unauthorized update, and duplicate initialization or invalid-state behavior.

Use local testing for the tight loop and devnet only for the demonstrated deployment. Record pinned tool versions because CLI/crate mismatches are a common classroom failure.
