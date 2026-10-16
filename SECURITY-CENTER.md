# Security Center

Status: proposed; not implemented or security-validated.

The UI is unprivileged and calls Guard's narrow API. It must distinguish desired policy, observed state, enforced state, and unknown/degraded state.

Navigation: Overview; Applications; Firewall; Storage & Files; Devices; Network; Identity & Secrets; System Integrity; Virtualization; Updates; Privacy; Developer Mode.

Show revocable grants, bounded permission history, listening services, blocked events, network profiles, and recovery readiness. Trusted camera/mic/screen-sharing indicators belong to a trusted shell/compositor, not an app overlay.

Administrative changes use scoped authorization. Lockdown is a transactional profile with clear consequences and recovery/management access safeguards. No UI-only claim of enforcement.
