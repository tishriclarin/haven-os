# Trusted interaction protocol

Status: proposed; not implemented or security-validated.

Only a trusted shell/compositor integration may issue gesture tokens. Synthetic app events, timestamps supplied by an app, and a button drawn by an app are insufficient.

Proposed token binding: cryptographic nonce, issuer, boot/session identity, verified app identity, action, resource-selection context, short expiry, and one-use consumption. Transport over authenticated local IPC; do not expose tokens in logs or command lines.

Consume atomically and reject replay, altered audience, other user/session, stale policy generation, and service restart. Authorize against current policy again before resource delivery.

Open question: trusted desktop integration and UX must be demonstrated before claiming gesture provenance. A generic desktop portal invocation alone is not proof of this property.
