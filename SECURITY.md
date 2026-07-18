# Security

Thanks for looking out for the tsvsheet family. If you believe you've found a vulnerability in any repository of this organization, please report it privately.

## Reporting

Use GitHub's private vulnerability reporting on the affected repository (Security → Report a vulnerability). Reports go directly to the maintainers; please don't open a public issue for a suspected vulnerability.

## What to expect

This is an open-source project maintained on a best-effort basis. We aim to acknowledge reports promptly, and validated issues are fixed with priority — releases are rebuilt from tagged source by CI, with checksums and build-provenance attestations you can verify (`gh attestation verify <file> --owner tsvsheet`). No service-level commitment, bounty, or guarantee is implied; the software is provided "as is" under each repository's MIT License.

## Scope notes

- The tsvsheet formula language is total by design: formulas cannot reach the network or the filesystem beyond confined sheet references, and hosts confine cross-sheet paths by default. Escapes from that confinement are exactly the kind of report we want.
- The playground and live sheets on tsvsheet.com run entirely in the browser; nothing you type is uploaded.
