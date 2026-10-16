# Security model

Status: proposed; not implemented or security-validated.

Combine least privilege, authenticated caller identity, trusted user authority, resource capabilities, kernel enforcement and VM compartmentalization.

Every sensitive operation needs a defined subject, object, action and authority. Enforce at the backend, not just in UI. Fail closed for new grants while preserving documented safe recovery behavior.

Review THREAT-MODEL.md, TRUST-MODEL.md and PERMISSION-MODEL.md together. A feature is not security-complete until its negative tests, crash behavior and limitations are documented.
