# Security Policy

## Reporting

Do not post credentials, financial account details, private legal documents, health information, private keys, recovery phrases, or personal identifiers in issues, commits, prompts, or screenshots. Stop work and notify Charles through a private approved channel if exposure is suspected.

## Required controls

- Use environment variables or an approved secret store.
- Commit only redacted examples such as `.env.example`.
- Apply least privilege and separate development from production.
- Validate inputs and outputs at every provider boundary.
- Log approvals and external writes without logging secrets.
- Require human approval for financial, legal, identity, publishing, and physical actions.
- Keep backups and a tested rollback path.
- Run dependency, secret, and static checks before deployment.

## AI-specific controls

Treat model output as untrusted input. Verify factual claims, code, citations, licensing, and instructions. Provider disagreements remain visible for review. Prompt content never overrides repository policy, owner authority, safety controls, or applicable law.

## Robotics and trading

Robotics work must remain simulated or supervised until safety gates pass. Trading code is research and paper-only by default; it must not accept broker credentials or submit live orders.

## Supported versions

This repository is pre-release. Security fixes apply to the current default branch.
