# Threat model

Status: proposed; not implemented or security-validated.

Protect user documents, identity, credentials, recovery material, policy integrity, and developer/management environments.

Adversaries include malicious apps, compromised dependencies, network attackers, hostile local networks, opportunistic device thieves, and malicious removable devices. Assume untrusted apps can send hostile IPC, race filesystem operations, and lie about their identity or UI.

Trusted base includes CPU/firmware assumptions, kernel/hypervisor, boot verification, trusted compositor, identity/authorization stack, and privileged brokers. A host kernel or trusted UI compromise can defeat this design.

Out of scope for the first prototype: guaranteed protection from malicious firmware or hardware implants, advanced physical/lab attacks, all side channels, denial of service, and a user intentionally granting access. VMs and Rust reduce specific risks; neither proves security.

Required abuse cases: token replay, confused deputy, forged caller, cross-user grant, symlink/rename race, daemon crash, audit exhaustion, malicious VM/device passthrough, poisoned update, and recovery loss. Each requires a test or an explicit documented limitation.
