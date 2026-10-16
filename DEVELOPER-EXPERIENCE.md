# Developer experience

Status: proposed; not implemented or security-validated.

Keep the host small. Build tools, dependency downloads, language servers, test databases, containers, and AI workloads run in dedicated VMs.

Share source through explicit reviewed transfer mechanisms; no default home mount or shared SSH agent. USB/GPU passthrough is resource-specific and visible. Disposable environments should be reproducible.

A Developer profile records exact exceptions, scope, duration, and restoration steps. It must not silently disable whole-host policy. Rust-first development does not justify replacing functioning upstream components without need.
