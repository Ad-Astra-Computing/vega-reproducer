# Security policy

The trust Vega provides depends on this reproducer behaving exactly as published,
so security reports are taken seriously.

## Reporting a vulnerability

Report privately through GitHub's private vulnerability reporting (the "Report a
vulnerability" button under the Security tab), or by email to
jason@adastracomputing.com. Do not open a public issue for a vulnerability.

Include the affected workflow, the conditions required to trigger it, and the
impact. A proof of concept helps. You will receive an acknowledgement within a
few days.

## Scope

This repository contains the reproduction workflow. It rebuilds untrusted Nix
code on a runner that can attest to Vega, so reports about the isolation between
an untrusted build and the attestation credential (the GitHub Actions OIDC token)
are especially in scope. The control plane and the agent are separate systems.
