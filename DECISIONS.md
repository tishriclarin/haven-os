# Decision log
Status is explicit. Architectural direction is accepted as project intent; details still require review.

| ID | Direction | Status |
|---|---|---|
| D001 | Debian Stable derivative; selective divergence | Accepted direction |
| D002 | Rust for new security-critical services | Accepted direction |
| D003 | TPM2, Secure Boot and LUKS2 secure profile | Accepted direction; boot policy open |
| D004 | Encrypted recovery exports and independent recovery drills | Accepted direction |
| D005 | KVM development boundary; rootless containers inside VMs | Accepted direction |
| D006 | No static host-folder grants to sandboxed apps | Accepted direction |
| D007 | User/policy-originated authority and trusted brokers | Accepted direction |
| D008 | Guard owns nftables policy; UI unprivileged | Accepted direction |
| D009 | Working name Haven OS and new SVG identity | Working; clearance/final approval open |
| D010 | MIT for original repository material | Initial repository default |
| D011 | IPC transport and trusted gesture issuer | Open |
| D012 | Revocable FD versus mediated file I/O | Open |
| D013 | Boot chain, PCR policy and anti-rollback | Open |

New ADRs must explain context, choice, alternatives, security impact, tests, and migration/recovery.
