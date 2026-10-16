# Execution plan
Status: proposed architecture; implementation has not begun.

## Phase 1 — Foundation
- [x] Establish public repository, mission, documentation, contributor guidance, and working SVG identity.
- [ ] Review threat model and identify the trusted computing base.
- [ ] Resolve token issuer, compositor integration, IPC transport, and caller identity.
- [ ] Specify broker protocols and capability lifecycle.
- [ ] Review boot, recovery, update rollback, and crash behavior.
- [ ] Approve MVP scope and record unresolved architecture decisions.

Exit gate: maintainer-reviewed architecture, documented limits, and executable test specifications. Documentation presence alone does not mean design approval.

## Phase 2 — Document capability MVP
Create Rust workspace; Guard policy engine; sandbox launcher; trusted chooser integration; document broker; one demo editor.
Acceptance:
1. Editor cannot enumerate host home, Documents, or Downloads.
2. App requests cannot manufacture trusted interaction or summon an authorization prompt.
3. One user gesture issues an app-, action-, session-, and object-bound single-use token.
4. One selected file is accessible with minimal mode; unrelated files remain inaccessible.
5. Deny, replay, expiry, restart, identity spoofing, and symlink/race tests fail closed.
6. Document exactly what revocation can stop; already read bytes cannot be recalled.
7. No host-wide policy changes or disk modifications in development tests.

## Phase 3 — Integration
Sensors/device brokers, permission history, per-app networking, nftables transactions, TPM/LUKS recovery, measured boot, and VM profiles.
Exit gate: integration tests in disposable VMs, recovery drills, adversarial review, and rollback validation.

## Phase 4 — Distribution prototype
Packaging, installer, signed repository, signed image, release provenance, and branded desktop.
Exit gate: independent installation/recovery testing and a published support/security policy.

## Work tracking
Use issues for owners, dependencies, evidence, and acceptance criteria. Update this file and decisions with behavior changes. Never claim an unfinished checkbox as an implemented feature.
