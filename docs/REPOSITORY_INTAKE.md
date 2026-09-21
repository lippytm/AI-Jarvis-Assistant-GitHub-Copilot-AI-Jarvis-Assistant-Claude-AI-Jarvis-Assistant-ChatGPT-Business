# Repository Intake and Growth Protocol

This protocol lets AI Jarvis expand across additional repositories without treating discovery as permission to operate.

## Intake states

1. **Quarantine / read-only** — inventory metadata, license, default branch, languages, existing workflows, secrets policy, open pull requests, and deployment surfaces.
2. **Classified** — assign a role, risk level, data sensitivity, owning Trust/LLC, and responsible human reviewer.
3. **Contracted** — add a work-item adapter, evidence format, health checks, and rollback instructions.
4. **Pilot** — make changes only on a feature branch and open a pull request. Use fixtures, sandboxes, paper trading, or simulation.
5. **Promoted** — enable a capability only after checks pass and the owner approves the exact scope.

## Automatic discovery versus authority

A repository appearing in `config/repositories.json` means only that Jarvis can see it. It does not authorize:

- merging or closing pull requests;
- deploying, publishing, or changing DNS;
- buying, selling, transferring, or custodying funds or assets;
- sending email, messages, contracts, or filings;
- creating or rotating production credentials;
- deleting data or disabling safeguards;
- commanding vehicles, wearables, robots, or other physical equipment.

Those actions require transaction-specific human approval and an auditable receipt.

## New-repository checklist

- [ ] Verify repository owner and intended Trust/LLC.
- [ ] Record the existing license; do not overwrite it.
- [ ] Scan for exposed credentials and remove them through an approved rotation process.
- [ ] Identify build, test, deploy, finance, legal, identity, and physical-system boundaries.
- [ ] Choose the smallest Jarvis adapter needed.
- [ ] Define expected inputs, outputs, provenance, and rollback.
- [ ] Add deterministic tests and a harmless round-trip test.
- [ ] Open a pull request; keep the default branch untouched.
- [ ] Obtain owner review before promotion.

## Creative growth lanes

Repositories can contribute ideas through governed work items in these lanes:

- software and AI systems;
- websites, publishing, film, music, and education;
- business operations and knowledge management;
- Web3 and market research in simulation or paper mode;
- robotics and wearables in simulation-first, supervised mode.

Creative proposals may flow freely as drafts. Real-world execution remains bounded by the platform policy, applicable law, safety review, and explicit human approval.

## Refresh procedure

When repositories are added:

1. rescan the authenticated GitHub installation;
2. append newly visible repositories as `quarantine-read-only`;
3. compare licenses and security posture;
4. propose classifications in a pull request;
5. never infer credentials or authority from repository names;
6. record evidence and the human decision that promotes a repository.
