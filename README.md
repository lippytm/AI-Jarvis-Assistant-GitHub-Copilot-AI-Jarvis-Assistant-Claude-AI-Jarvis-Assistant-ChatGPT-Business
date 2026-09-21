# AI Jarvis Assistant — Unified Systems Hub

This repository is the coordination layer for AI Jarvis Assistant across GitHub Copilot, ChatGPT/ChatGPT Business, Claude, Gemini, Hostinger, websites, and approved business systems.

## Purpose

- Define one portable work-item contract for every AI platform.
- Preserve provenance, approvals, ownership, and audit history.
- Keep Charles Earl Lipshay as final human authority.
- Separate planning and recommendations from external execution.
- Provide reusable validation and security controls for other repositories.

## Operating model

1. **Intake** — register the project, owning Trust/LLC, source, objective, constraints, and sensitivity.
2. **Plan** — create measurable deliverables and acceptance tests.
3. **Build** — work on a branch; do not expose secrets or overwrite unrelated work.
4. **Review** — QA, security, licensing, accessibility, and factual checks.
5. **Approve** — Charles or a named authorized human approves external or high-impact actions.
6. **Deploy** — controlled release with logs, rollback, and post-deployment verification.
7. **Learn** — record outcomes and reusable improvements without silently changing authority or risk limits.

## Repository map

- `docs/ARCHITECTURE.md` — system boundaries and integration pattern.
- `config/platforms.json` — declared platform capabilities and prohibited behavior.
- `schemas/work-item.schema.json` — portable project handoff format.
- `SECURITY.md` — secrets, privacy, incident, and safety rules.
- `.github/workflows/validate.yml` — JSON and Python syntax validation.

## Authority boundaries

Jarvis may research, draft, compare, test, report, and recommend. Jarvis may not independently sign contracts, file legal documents, invest or transfer real money, borrow, publish private data, change ownership, deploy unsafe robotics, or bypass a failed quality gate.

Trading integrations remain paper-only unless Charles provides separate written authorization after legal, tax, security, and risk review. Robotics follows simulation → isolated bench → emergency-stop verification → supervised trial → QA certification → controlled deployment.

## License notice

The repository currently includes a CC0 license selected before this foundation. This pull request does not change it. Because the broader portfolio also discusses proprietary code, creative-content, and commercial terms, the final licensing strategy requires owner and qualified-attorney review before valuable IP is added or mirrored.

## First integration targets

1. AI Jarvis control-plane and self-healing repositories.
2. Hostinger and aievolutionaryevolutions.com integration.
3. Claude/Gemini/ChatGPT handoff packets.
4. Prompt #11 publishing, CRM, video, education, and Idea Ledger projects.
5. Trading research and robotics planning as isolated, gated systems.
