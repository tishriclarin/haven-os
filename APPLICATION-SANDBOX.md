# Application sandbox

Status: proposed; not implemented or security-validated.

Use kernel-enforced namespaces, restricted mounts, device filtering, syscall policy, resource limits, and selected LSM controls. Flatpak may be an integration base, but its defaults do not automatically satisfy Haven's stricter authority model.

No broad home mount, host socket, privileged container flag, or unrestricted device escape hatch. Private app state is distinct from shared user documents. App identity must survive launch, update, and IPC verification.

Demonstrate isolation in disposable VMs before expanding app compatibility. Landlock/AppArmor availability and stacking must be probed and tested; do not describe unverified combinations as enforced.
