# Week 7 — Reference solution

Use one transaction lifecycle: `draft → simulating → awaiting-signature → submitted → confirmed`, with explicit failure transitions. Render the signature only after submission and success only after confirmation.

Keep cluster/program configuration centralized. Decode state only after checking expected program owner and schema/discriminator. Refresh reads after confirmation.

The quality bar is a reproducible flow and honest error handling, not visual complexity.
