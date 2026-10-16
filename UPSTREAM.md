# Upstream policy

Status: proposed; not implemented or security-validated.

Debian Stable supplies the base. Prefer upstream fixes and narrow patches; fork only when required by the reviewed security model.

| Component | Intended classification |
|---|---|
| Kernel, libc, systemd, apt/dpkg, libraries | Upstream unmodified initially |
| Guard, capability protocol, Security Center | Haven-only |
| Desktop portal and trusted shell integration | Evaluate patched/forked/replaced |
| Installer, boot and update integration | Integration first; divergence by ADR |

Track version, source, patches, license, security owner and update lag for every divergence. No Debian packages are vendored in this foundation commit.
