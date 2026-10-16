# VM security

Status: proposed; not implemented or security-validated.

KVM/QEMU VMs are the primary boundary for development and untrusted workloads. Containers share a kernel and belong inside development VMs, preferably rootless. No development Docker daemon/socket on the trusted host.

Profiles: management, Rust/backend development, Android development, network lab, AI, untrusted. Default: no host filesystem, clipboard, shared credential agent, or unmanaged USB access; explicit Internet-only networking as needed.

GPU passthrough needs IOMMU isolation, group/reset checks, and an independently usable host display. A device bound to vfio must not simultaneously use the host NVIDIA driver. Do not ban host GPU drivers globally when no passthrough is used.

VM escapes, side channels and device flaws remain risks. Snapshot state and VM secrets require encryption and lifecycle rules.
