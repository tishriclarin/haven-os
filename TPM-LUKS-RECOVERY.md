# TPM, LUKS and recovery

Status: proposed; not implemented or security-validated.

Secure profile: TPM2, LUKS2, verified boot, and independently tested recovery. PCR policy and enrollment procedure remain design decisions; do not hardcode a universal PCR recipe.

Record expected boot measurements and policy transitions. Secure Boot authenticates configured signatures; measurement and attestation are distinct. A green UI requires verified evidence, not mere TPM presence.

Store/export recovery material only in encrypted form with independently protected decryption credentials. Recovery necessarily handles secrets in trusted memory; never log them. Maintain an offline tested recovery route independent of the TPM and host.

Before reenrollment, firmware changes, or keyslot removal: verify backup, test recovery, document current policy, and provide rollback. Boot updates must not silently brick auto-unlock. A recovery drill is a release gate.
