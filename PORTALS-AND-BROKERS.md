# Portals and brokers

Status: proposed; not implemented or security-validated.

Session brokers translate approved user intent into narrow resource operations. Apps may describe a need, but cannot independently cause an authorization UI to grant authority.

Document MVP: trusted action selects file; broker resolves object safely; policy checks requested mode; broker delivers an FD or mediated handle to the verified app. Avoid path-only authorization and check/use races.

Define typed request/response schemas, limits, cancellation, timeouts, error behavior, and audit fields before coding. Never broker arbitrary commands, host paths, or secrets by default. Resource-specific brokers isolate parsing and privileges.
