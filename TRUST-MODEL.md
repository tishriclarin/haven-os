# Trust and authority

Status: proposed; not implemented or security-validated.

Authority originates from explicit policy or a real user action captured by trusted system components. An application request is data, never proof of consent.

The trusted shell issues narrowly scoped interaction evidence; a broker validates freshness, caller binding, target operation, session, and consumption. Guard decides whether policy permits the operation. Administrative authorization is separate from login.

Root and the kernel remain powerful trusted actors. This model does not claim isolation against a fully compromised host. Permission dialogs must identify the verified caller and consequence, not display arbitrary app-supplied text as trusted truth.
