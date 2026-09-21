# Unified Jarvis Architecture

## Components

- **Control plane:** project registry, policies, approvals, routing, and status.
- **Work-item envelope:** portable JSON containing identity, ownership, provenance, task state, evidence, and acceptance tests.
- **Provider adapters:** translate the envelope for ChatGPT, Claude, Gemini, GitHub Copilot, Hostinger, or another approved platform.
- **Evidence store:** source references, hashes, test output, decisions, and audit events.
- **RiskGate:** blocks actions lacking owner approval, credentials, safety evidence, or legal authority.
- **QA/Whistleblower lane:** independently records defects and may stop work.
- **Deployment adapters:** repository PRs, website staging, document publication, and future supervised robotics interfaces.

## Event flow

```text
Intake -> Ownership check -> Risk classification -> Plan -> Build branch
       -> Automated validation -> Human/QA review -> Charles approval
       -> Controlled deployment -> Verification -> Audit record
```

## Cross-platform contract

Every provider receives the same work-item ID and must return:

- provider name and model/tool version when available;
- input artifact hashes or immutable references;
- proposed changes and files affected;
- tests performed and evidence produced;
- unresolved risks, assumptions, and requested approvals;
- a handoff status: `draft`, `blocked`, `review`, `approved`, or `complete`.

Provider output is advisory until reconciled into the authoritative GitHub work item. Conflicting answers are preserved and reviewed; they are not silently merged.

## Security boundaries

- Secrets stay in approved secret stores and are never committed.
- Production and personal accounts are isolated from development.
- External writes are least-privilege and logged.
- Financial, legal, medical, identity, and physical-safety actions require human approval.
- Fail closed when credentials, ownership, scope, or policy is ambiguous.
- A rollback path is required before deployment.

## Portfolio integration

The hub coordinates rather than copying every project into one repository. Each project remains independently versioned and links back through a work-item ID, owning entity, dependency list, and release evidence.
