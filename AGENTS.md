Read AGENTS-shape.md first — the rules of this repository's shape.

This is the assembly root of **openSig** (`opensig`): the repository an
engineer clones. It holds `project.yaml`, the pins and the gate, and it mounts
the two legs.

| role | repository | path |
|---|---|---|
| assembly | `opensoft/openSig` | `.` |
| spec | `opensoft/openSig-spec` | `spec/` |
| code | `opensoft/openSig-code` | `code/` |

Everything below this line is openSig's own. The shape wrote the block above
once and does not pin this file, so how this project is built, tested, reviewed
and released belongs here and nothing upstream will overwrite it.

## openSig project rules

All original project work is Apache-2.0. Third-party shipped code, assets and dependencies must pass an MIT/Apache license allowlist. Never commit real patient data, signature images, credentials, private keys or wallet secrets. Use synthetic fixtures.

Keep clinical attestation and amendments in openChart, financial authority in openPractice, and human personal approval outside Hermes service credentials. Optional anchoring publishes commitments only and does not block ordinary signing.

Use the shared user-level OpenSpec/Speckit protocol. Canonical governance and feature plans live in the spec leg; implementation and tests live in the code leg. Shape rules live in the assembly root's AGENTS-shape.md. No signing runtime/test commands exist yet; establish them with the first governed implementation.
