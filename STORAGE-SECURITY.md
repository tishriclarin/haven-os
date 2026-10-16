# Storage security

Status: proposed; not implemented or security-validated.

Secure installation profile requires LUKS2 for system/user persistent storage; boot partition handling depends on the chosen verified-boot chain. Separate system, user, app, and VM state.

TPM auto-unlock is convenience with policy binding, not a substitute for login or recovery. Protect keys and backups, minimize unlock material lifetime, and require deliberate authorization for recovery export.

Snapshots are not backups. LVM snapshots are capacity-limited and can become invalid; rollback must coordinate boot artifacts, package database, configuration, and data schema versions. Never issue destructive storage operations without verified device identity and recovery prerequisites.
