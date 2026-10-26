# Private Developer Alpha release records

This directory contains non-secret provenance records for the invitation-only
Developer Alpha channel. Package bytes are never committed here and no public
download URL is recorded. The private delivery path is:

```text
verified ZIP → private Cloudflare R2 object → Supabase alpha_release_assets
             → authenticated Worker → approved developer portal
```

Each asset must be registered with its exact source commit, platform,
architecture, filename, byte size, SHA-256 checksum, and trust-evidence
reference before its Supabase availability is changed to `available`.

The offline license signer runs locally on the owner’s macOS machine. Its
private Ed25519 seed remains in macOS Keychain; this repository may contain
only the public key identifier and public key after key generation.

Do not add ZIP files, R2 credentials, Supabase service keys, signer tokens,
installation identities, contact details, or license signatures for real users
to this repository.
