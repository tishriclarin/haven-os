# Permission model

Status: proposed; not implemented or security-validated.

Default: private app storage only; no host home/Documents/Downloads mount, no camera/mic/USB/secrets access, and no implicit LAN or Internet authority.

A grant records subject identity, user/session, resource identity, permitted operations, issuing authority, creation/expiry, policy generation, and revocation state. Persistent exceptions require explicit administrative/user policy and visible indicators.

Internet and LAN are distinct. Files, sensors, clipboard, screen capture, notifications, background execution, and secrets use independent policy scopes.

Revocation denies future broker operations. Open file descriptors and copied data cannot generally be recalled; strict revocation may require mediated I/O or terminating the workload. The UI must accurately distinguish policy revoked from all access stopped.
