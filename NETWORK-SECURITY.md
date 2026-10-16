# Network security

Status: proposed; not implemented or security-validated.

Guard owns the policy model; nftables is an enforcement backend. Apply validated transactions atomically, test syntax before activation, and preserve a known-good policy.

Per-app networking requires enforceable identity such as controlled namespaces/cgroups and managed launch. nftables alone does not reliably turn arbitrary processes into verified desktop app identities. Cover IPv4, IPv6, DNS, loopback, multicast, raw sockets, and namespace escape paths.

Profiles: Trusted, Home, Work, Public, Untrusted. Public/Untrusted deny inbound, LAN and discovery by default. A network name/SSID alone is not trusted authentication.

Live blocked events are bounded and rate limited. Minimize destination retention; no payload logging. Show listening services and enforcement degradation. Developer exceptions must be scoped and visible.
