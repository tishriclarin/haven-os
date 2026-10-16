# Updates and rollback

Status: proposed; not implemented or security-validated.

Use upstream security updates with documented integration tests and a separately signed Haven repository. Verify metadata, artifacts and release provenance. Protect signing keys outside ordinary build jobs and define key rotation/revocation.

Transactional deployment is a goal. Initially evaluate snapshot-assisted updates; later evaluate signed images/read-only usr or A/B deployment. Rollback must include boot, root filesystem and compatible data schemas.

An old signed vulnerable image remains a risk. Define anti-rollback policy and emergency recovery exceptions before production. Test interrupted update, low disk, invalid signature, failed boot and TPM policy transitions.
