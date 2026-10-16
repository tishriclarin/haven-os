# AI project context
Haven OS is a documentation-first Debian-derived privacy OS project, not a production distro. Rust is intended for new security-critical services.

Read AGENTS.md and AI_RULES.md, then PLANS.md and relevant models. Trusted user interaction or explicit policy grants authority; app requests alone cannot. Sandbox apps lack broad host folder access. Guard owns policy; brokers provide narrow resources; UI stays unprivileged.

TPM2/LUKS2 secure profile, encrypted recovery export, VM-first development and nftables integration are planned. Existing Linux mechanisms do not automatically provide every desired capability. Identify gaps honestly.

Current task scope is foundation architecture. Do not partition disks, alter boot, enroll keys, change host firewall or claim an implemented security feature without explicit task scope and validation.
